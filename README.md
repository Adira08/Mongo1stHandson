<h1>Question1:Create a database , give it name like "Human_Resource".</h1>
    <p>use Human_Resource <br>
        switched to db Human_Resource</p>

<h1>Question2:Create a collection inside this named "employee"</h1>
    <p>Human_Resource> db.createCollection("employee"); <br>
        { ok: 1 }</p>
    
 <h1>Question3:Query the collection "employee" and list all the documents.</h1>
    <p>Link:https://prepbytes-misc-images.s3.ap-south-1.amazonaws.com/assets/1640781204638-employee.json</p>
    <code>
        <pre>
            Human_Resource> db.employee.insertMany([{
                ...   "firstName": "John",
                ...   "lastName": "Doe",
                ...   "salary": "25000",
                ...   "department": "HR",
                ...   "lastCompany": "X",
                ...   "lastSalary": "10000",
                ...   "overallExp": "2",
                ...   "contactInfo": "1234567890",
                ...   "yearGrad": "2016",
                ...   "gradStream": "CSE"
                ... },
                ... {
                ...   "firstName": "Rohan",
                ...   "lastName": "Jame",
                ...   "salary": "30000",
                ...   "department": "Technical",
                ...   "lastCompany": "Y",
                ...   "lastSalary": "15000",
                ...   "overallExp": "1",
                ...   "contactInfo": "1234567860",
                ...   "yearGrad": "2015",
                ...   "gradStream": "CSE"
                ... },
                ... {
                ...  "firstName": "Jame",
                ...   "lastName": "Doe",
                ...   "salary": "35000",
                ...   "department": "Accounts",
                ...   "lastCompany": "Z",
                ...   "lastSalary": "20000",
                ...   "overallExp": "1",
                ...   "contactInfo": "123567890",
                ...   "yearGrad": "2019",
                ...   "gradStream": "ECE"
                ... },
                ... {
                ...  "firstName": "Sao",
                ...   "lastName": "Avika",
                ...   "salary": "30000",
                ...   "department": "Sales",
                ...   "lastCompany": "Y",
                ...   "lastSalary": "15000",
                ...   "overallExp": "2",
                ...   "contactInfo": "1234567860",
                ...   "yearGrad": "2015",
                ...   "gradStream": "CSE"
                ... },
                ... {
                ...  "firstName": "Jame",
                ...   "lastName": "roh",
                ...   "salary": "35000",
                ...   "department": "Accounts",
                ...   "lastCompany": "Z",
                ...   "lastSalary": "15000",
                ...   "overallExp": "2",
                ...   "contactInfo": "123567890",
                ...   "yearGrad": "2019",
                ...   "gradStream": "EEE"
                ... },
                ... {
                ...   "firstName": "Rohan",
                ...   "lastName": "Jame",
                ...   "salary": "30000",
                ...   "department": "Technical",
                ...   "lastCompany": "Y",
                ...   "lastSalary": "15000",
                ...   "overallExp": "1",
                ...   "contactInfo": "1234567860",
                ...   "yearGrad": "2015",
                ...   "gradStream": "CSE"
                ... },
                ... {
                ...    "firstName": "Jame",
                ...   "lastName": "Doe",
                ...   "salary": "35000",
                ...   "department": "Accounts",
                ...   "lastCompany": "Z",
                ...   "lastSalary": "20000",
                ...   "overallExp": "1",
                ...   "contactInfo": "123567890",
                ...   "yearGrad": "2019",
                ...   "gradStream": "ECE"
                ... },
                ... {
                ...   "firstName": "Sao",
                ...   "lastName": "Avika",
                ...   "salary": "30000",
                ...   "department": "Sales",
                ...   "lastCompany": "Y",
                ...   "lastSalary": "15000",
                ...   "overallExp": "2",
                ...   "contactInfo": "1234567860",
                ...   "yearGrad": "2015",
                ...   "gradStream": "CSE"
                ... },
                ... {
                ...   "firstName": "Jame",
                ...   "lastName": "Doe",
                ...   "salary": "35000",
                ...   "department": "Accounts",
                ...   "lastCompany": "Z",
                ...   "lastSalary": "15000",
                ...   "overallExp": "2",
                ...   "contactInfo": "123567890",
                ...   "yearGrad": "2019",
                ...   "gradStream": "EEE"
                ... },
                ... {
                ...   "firstName": "Rohan",
                ...   "lastName": "Jame",
                ...   "salary": "30000",
                ...   "department": "Technical",
                ...   "lastCompany": "Y",
                ...   "lastSalary": "15000",
                ...   "overallExp": "1",
                ...   "contactInfo": "1234567860",
                ...   "yearGrad": "2015",
                ...   "gradStream": "CSE"
                ... },
                ... {
                ...   "firstName": "Jame",
                ...   "lastName": "Doe",
                ...   "salary": "35000",
                ...   "department": "Accounts",
                ...   "lastCompany": "Z",
                ...   "lastSalary": "20000",
                ...   "overallExp": "1",
                ...   "contactInfo": "123567890",
                ...   "yearGrad": "2019",
                ...   "gradStream": "ECE"
                ... },
                ... {
                ...   "firstName": "Sao",
                ...   "lastName": "Avika",
                ...   "salary": "30000",
                ...   "department": "Sales",
                ...   "lastCompany": "Y",
                ...   "lastSalary": "15000",
                ...   "overallExp": "2",
                ...   "contactInfo": "1234567860",
                ...   "yearGrad": "2015",
                ...   "gradStream": "CSE"
                ... },
                ... {
                ...   "firstName": "Jame",
                ...   "lastName": "Doe",
                ...   "salary": "35000",
                ...   "department": "Accounts",
                ...   "lastCompany": "Z",
                ...   "lastSalary": "15000",
                ...   "overallExp": "2",
                ...   "contactInfo": "123567890",
                ...   "yearGrad": "2019",
                ...   "gradStream": "EEE"
                ... }]);
        </pre>
    </code>
    <code>
        <pre>
            {
                acknowledged: true,
                insertedIds: {
                  '0': ObjectId("637f7c7b785b96df93b9380d"),
                  '1': ObjectId("637f7c7b785b96df93b9380e"),
                  '2': ObjectId("637f7c7b785b96df93b9380f"),
                  '3': ObjectId("637f7c7b785b96df93b93810"),
                  '4': ObjectId("637f7c7b785b96df93b93811"),
                  '5': ObjectId("637f7c7b785b96df93b93812"),
                  '6': ObjectId("637f7c7b785b96df93b93813"),
                  '7': ObjectId("637f7c7b785b96df93b93814"),
                  '8': ObjectId("637f7c7b785b96df93b93815"),
                  '9': ObjectId("637f7c7b785b96df93b93816"),
                  '10': ObjectId("637f7c7b785b96df93b93817"),
                  '11': ObjectId("637f7c7b785b96df93b93818"),
                  '12': ObjectId("637f7c7b785b96df93b93819")
                }
              }
        </pre>
    </code>

   <code><pre>
        Human_Resource> db.employee.find().pretty();
    </pre></code>
    <code><pre>
        [{ _id: ObjectId("637f7c7b785b96df93b9380d"),
        firstName: 'John',
        lastName: 'Doe',
        salary: '25000',
        department: 'HR',
        lastCompany: 'X',
        lastSalary: '10000',
        overallExp: '2',
        contactInfo: '1234567890',
        yearGrad: '2016',
        gradStream: 'CSE' 
        }
        { _id: ObjectId("637f7c7b785b96df93b9380e"),
        firstName: 'Rohan',
        lastName: 'Jame',
        salary: '30000',
        department: 'Technical',
        lastCompany: 'Y',
        lastSalary: '15000',
        overallExp: '1',
        contactInfo: '1234567860',
        yearGrad: '2015',
        gradStream: 'CSE'
         },
        { _id: ObjectId("637f7c7b785b96df93b9380f"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '20000',
        overallExp: '1',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'ECE'
         },
        { _id: ObjectId("637f7c7b785b96df93b93810"),
        firstName: 'Sao',
        lastName: 'Avika',
        salary: '30000',
        department: 'Sales',
        lastCompany: 'Y',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '1234567860',
        yearGrad: '2015',
        gradStream: 'CSE' 
        },
        { _id: ObjectId("637f7c7b785b96df93b93811"),
        firstName: 'Jame',
        lastName: 'roh',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'EEE' }
        { _id: ObjectId("637f7c7b785b96df93b93812"),
        firstName: 'Rohan',
        lastName: 'Jame',
        salary: '30000',
        department: 'Technical',
        lastCompany: 'Y',
        lastSalary: '15000',
        overallExp: '1',
        contactInfo: '1234567860',
        yearGrad: '2015',
        gradStream: 'CSE' 
        },
        { _id: ObjectId("637f7c7b785b96df93b93813"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '20000',
        overallExp: '1',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'ECE' }
        { _id: ObjectId("637f7c7b785b96df93b93814"),
        firstName: 'Sao',
        lastName: 'Avika',
        salary: '30000',
        department: 'Sales',
        lastCompany: 'Y',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '1234567860',
        yearGrad: '2015',
        gradStream: 'CSE' }
        { _id: ObjectId("637f7c7b785b96df93b93815"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'EEE'
         },
        { _id: ObjectId("637f7c7b785b96df93b93816"),
        firstName: 'Rohan',
        lastName: 'Jame',
        salary: '30000',
        department: 'Technical',
        lastCompany: 'Y',
        lastSalary: '15000',
        overallExp: '1',
        contactInfo: '1234567860',
        yearGrad: '2015',
        gradStream: 'CSE' }
        { _id: ObjectId("637f7c7b785b96df93b93817"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '20000',
        overallExp: '1',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'ECE' 
        },
        { _id: ObjectId("637f7c7b785b96df93b93818"),
        firstName: 'Sao',
        lastName: 'Avika',
        salary: '30000',
        department: 'Sales',
        lastCompany: 'Y',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '1234567860',
        yearGrad: '2015',
        gradStream: 'CSE' }
        { _id: ObjectId("637f7c7b785b96df93b93819"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'EEE' 
        },]
        </pre></code>

<h1>Question4:Query the collection "employee" and list the employees who are having salary more than 30000.</h1>
    <p>Human_Resource> db.employee.find({"salary" : {$gt:"30000"}});</p>
    <code><pre>     
        [{ _id: ObjectId("637f7c7b785b96df93b9380f"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '20000',
        overallExp: '1',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'ECE' 
        },
        { _id: ObjectId("637f7c7b785b96df93b93811"),
        firstName: 'Jame',
        lastName: 'roh',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'EEE' 
        },
        { _id: ObjectId("637f7c7b785b96df93b93813"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '20000',
        overallExp: '1',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'ECE' 
        },
        { _id: ObjectId("637f7c7b785b96df93b93815"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'EEE' 
        },
        { _id: ObjectId("637f7c7b785b96df93b93817"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '20000',
        overallExp: '1',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'ECE' 
        },
        { _id: ObjectId("637f7c7b785b96df93b93819"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'EEE'
        },]
    </pre></code>

<h1>Question5:Query the collection "employee" and list the employees who are having experience more than 2 years.</h1>
    <p>
        Human_Resource> db.employee.find({"overallExp" : {$gt:"2"}}); <br>
        Comment:As no data is available whose experience is greater than 2 years.
    </p>
    <h1>Question6:Query the collection "employee" and list the employees who are graduated after 2015 and having experience more than 1 year.</h1>
    <p>Human_Resource> db.employee.find({yearGrad:{$gt:"2015"},overallExp:{$gt:"1"}});</p>
    <code><pre>
        [_id: ObjectId("637f7c7b785b96df93b9380d"),
        firstName: 'John',
        lastName: 'Doe',
        salary: '25000',
        department: 'HR',
        lastCompany: 'X',
        lastSalary: '10000',
        overallExp: '2',
        contactInfo: '1234567890',
        yearGrad: '2016',
        gradStream: 'CSE' 
        },
        { _id: ObjectId("637f7c7b785b96df93b93811"),
        firstName: 'Jame',
        lastName: 'roh',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'EEE'
        },
        { _id: ObjectId("637f7c7b785b96df93b93815"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'EEE' }
        { _id: ObjectId("637f7c7b785b96df93b93819"),
        firstName: 'Jame',
        lastName: 'Doe',
        salary: '35000',
        department: 'Accounts',
        lastCompany: 'Z',
        lastSalary: '15000',
        overallExp: '2',
        contactInfo: '123567890',
        yearGrad: '2019',
        gradStream: 'EEE' 
        },]
    </pre></code>

<h1>Question7:Query the collection "employee" and update the salary of the employee whose salary is greater than 70000 to 65000.</h1>
    <p>Human_Resource> db.employee.updateMany({"salary":{$gt:"70000"}},{$set:{"salary":"65000"}});</p>
    <code><pre>
        {
            acknowledged: true,
            insertedId: null,
            matchedCount: 0,
            modifiedCount: 0,
            upsertedCount: 0
          }
    </pre></code>

<h1>Question8:Delete all the documents from "employee" where last company is Y.</h1>
    <p>Human_Resource> db.employee.deleteMany({"lastCompany":"Y"}); <br>
        { acknowledged: true, deletedCount: 6 }</p>
