# Learning about JsonPower DB
JsonPowerDB is a Database Server with Developer friendly REST API services. It's a High Performance, Light Weight, Ajax Enabled, Serverless, Simple to Use, Real-time Database.
Easy and fast to develop database applications without using any server side programming / scripting or without installing any kind of database.

## Benefits of JsonPower DB
### JsonPowerDB (JPDB) is Next Generation, Creative and Disruptive Multi-mode DBMS_ with many USPs.

1.Proprietary algorithm for High Performance CRUD operations. Multiple times faster than popular DBMS

2.Serverless support for faster development - A UI developer can develop complete dynamic application.

3.DBMS with built in web / application server and embedded caching makes the performance lightning fast.

4.Server side Native NoSQL - best query performance.

5.In-built support to query on multiple JPDB databases.

6.Multi-mode DBMS - Document DB, Key-Value DB, RDBMS support.

7.Schema free - easy to develop and maintain.

8.Web-services API - Can be used with any programming language that has support for HTTP.

9.Enriched by a pluggable API Framework - A developer can develop a pluggable API and plugin into any of our cloud JPDB instance.

10.Standardisation of API development framework makes the development process easy, more readable, and less error prone.

11.Multiple security layers.

12.Nimble, Simple to use, In Memory, Real-time DBMS.

## JsonPowerDB code

## IN IML commands
### PUT
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "PUT",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "jsonStr": {
		
        "name": "vishali",
				
        "email": "vishalini@login2explore.com",
				
      "mobile":3456789023
			
    }
		
}



### PUT_ALL

{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "PUT_ALL",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "templateStr": {},
		
    "colsAutoIndex": true,
		
    "jsonStr": [
		
        {
				
            "name": "Pranitha",
						
            "email": "pranitha@gmail.com",
						
            "password": "3293",
						
            "password": "3293"

        },
				
        {
				
            "name": "Sarah Khan",
						
            "email": "sarahkhan@gmail.com",
						
            "password": "3823",
						
            "passwrd": "3823"
						

        },
				
        {
				
            "name": "Akhil",
						
            "email": "akhil81@gmail.com",
						
            "password": "3273",
						
						
            "passwrd": "3273"

        }
				
    ]
		
}


### UPDATE

{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "UPDATE",
		
    "dbName": "Employee",
		
	"rel": "Emp-Rel",
		
    "jsonStr": {
		
       "1":{
			 
        "mobile": 2345234567
				
      },
			
       "2":{
			 
        "name": "vishalini nandakumar"
				
          "mobile": 2341222234
					
      }
			
   }
	 
}

### DELETE

{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "REMOVE",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "record": 1
		
}
## In IRL commands
### GET : Retrieve single record by json data (Deprecated use GET_BY_KEY instead of GET)
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "GET",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "jsonStr": {
		
        "name": "vishali"
				
    }
		
}
### GET_BY_KEY : Retrieve single record by json data
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "GET_BY_KEY",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "createTime": true,
	 
    "updateTime": true,
		
    "jsonStr": {
		
        "name": "vishali"
				
    }
		
}

### GET_ALL : Retrieve multiple records from relation
{

    "token": "90935796|-31948838699886563|90934728",
		
    "dbName": "Employee",
		
    "cmd": "GET_ALL",
		
    "rel": "Emp-Rel",
		
    "pageNo": 1,
		
    "pageSize": 5,
		
    "createTime": true,
		
    "updateTime": true
}


### SYNC_DB : Retrieve updated multiple records from multiple relations using timestamp
{

    "token": "90935796|-31948838699886563|90934728",
		
    "dbName": "Employee",
		
    "cmd": "SYNC_DB",
		
    "relTsJson": {
		
        "password": 0
    },
		
    "createTime": true,
		
    "updateTime": true
		
}   

### FIND_RECORD/FIND_ALL_RECORD : Retrieve records by json data
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "FIND_ALL_RECORDS",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "jsonStr": {
		
         "mobile":3456789023
				 
    },
		
    "createTime": true,
 
    "updateTime": true
		

}

### GET_RECORD : Retrieve single record by record number (Deprecated now use GET_BY_RECORD)
{

    "token": "90935796|-31948838699886563|90934728",
		
     "cmd": "GET_RECORD",
		 
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "record": 11
		
}

### GET_BY_RECORD : Retrieve single record by record number
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "GET_BY_RECORD",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "record": 11
		
      "createTime": true,
			
    "updateTime": true
		
}

### FIRST_RECORD : Retrieve first record from the JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "FIRST_RECORD",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "createTime": true,
		
    "updateTime": true
		
}

### LAST_RECORD : Retrieve last record from the JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "LAST_RECORD",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "createTime": true,
		
    "updateTime": true
		
}

### NEXT_RECORD : Retrieve next record by record number
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "NEXT_RECORD",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "record": 2,
		
    "createTime": true,
		
    "updateTime": true
		
}

### PREV_RECORD : Retrieve previous record by record number
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "PREV_RECORD",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel",
		
    "record": 12,
		
    "createTime": true,
		
    "updateTime": true
		
}

### GET_RELATION_STATS / GET_RELATION_SIZE : Get total number of records and size of relation
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "GET_RELATION_STATS",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel"
		
}

### GET_ALL_DB : Retrieve all database names from JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "GET_ALL_DB"
		
}

### GETALLREL : Retrieve all relation details from JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "GETALLREL"
		
    "dbName": "Employee"
		
}

### GET_INDEXED_COL : Retrieve all indexed column names from JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "GET_INDEXED_COL"
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel"
		
}

### GET_NON_INDEXED_COL : Retrieve all non indexed column names from JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "GET_NON_INDEXED_COL"
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel"
		
}
### GET_ALL_COL : Retrieve all column names from JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "GET_ALL_COL"
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel"
		
}

### IS_COLUMN_INDEXED : Check whether a column is indexed or not
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "IS_COLUMN_INDEXED"
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel"
		
    "colName": "email"
		
}

### IS_COLUMN_EXIST : Check whether a column exist or not in the JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "IS_COLUMN_EXIST"
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel"
		
    "colName": "email"
		
}
### IS_RELATION_EXIST : Check whether a Relation exist or not in the JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "IS_RELATION_EXISTS",
		
    "dbName": "Employee",
		
    "rel": "Emp-Rel"

}

### IS_DATABASE_EXIST : Check whether a Database exist or not in the JPDB database
{

    "token": "90935796|-31948838699886563|90934728",
		
    "cmd": "IS_DATABASE_EXISTS",
		
    "dbName": "Employee"
		
}
## overview of Talend API tester
<img src="https://user-images.githubusercontent.com/66720092/110650507-9eb12900-81e0-11eb-8ae1-3663cdb6edc0.jpg" width="1000">

## in jsonPower DB

<img src="https://user-images.githubusercontent.com/66720092/110651656-a45b3e80-81e1-11eb-9740-376213a2b450.jpg" width="1000">
<img src="https://user-images.githubusercontent.com/66720092/110651739-bb9a2c00-81e1-11eb-9f05-613b8d734eb1.jpg" width="1000">

## overview of JsonPower DB

### CODE 
<!DOCTYPE html>
<!--
To change this license header, choose License Headers in Project Properties.
To change this template file, choose Tools | Templates
and open the template in the editor.
-->
<html lang="en">
    <head>
        <title>Bootstrap Example</title>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link rel="stylesheet"
              href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
        <script
        src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
        <script
        src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
        
    </head>
    <body>
        <div class="container">
            <h2>Vertical (basic) form</h2>
            <form id="empForm" method="post">
                <div class="form-group">
                    <span><label for="empId">Employee ID:</label> <label id="empIdMsg">
                        </label></span>
                    <input type="text" class="form-control" name="empId" id="empId"
                           placeholder="Enter Employee ID" required>
                </div>
                <div class="form-group">
                    <label for="empName">Employee Name:</label>
                    <input type="text" class="form-control" id="empName"
                           placeholder="Enter Employee Name" name="empName">
                </div>
                <div class="form-group">
                    <label for="empEmail">Email:</label>
                    <input type="email" class="form-control" id="empEmail"
                           placeholder="Enter Employee Email" name="empEmail">
                </div>
                <input type="button" class="btn btn-primary" id="empSave" value="Save"
                       onclick="saveEmployee();">
            </form>
        </div>
        <script>
            $("#empId").focus();
            function validateAndGetFormData() {
                var empIdVar = $("#empId").val();
                if (empIdVar === "") {
                    alert("Employee ID Required Value");
                    $("#empId").focus();
                    return "";
                }
                var empNameVar = $("#empName").val();
                if (empNameVar === "") {
                    alert("Employee Name is Required Value");
                    $("#empName").focus();
                    return "";
                }
                var empEmailVar = $("#empEmail").val();
                if (empEmailVar === "") {
                    alert("Employee Email is Required Value");
                    $("#empEmail").focus();
                    return "";
                }
                var jsonStrObj = {
                    empId: empIdVar,
                    empName: empNameVar,
                    empEmail: empEmailVar,
                };
                return JSON.stringify(jsonStrObj);
            }
// This method is used to create PUT Json request.

            function createPUTRequest(connToken, jsonObj, dbName, relName) {
                var putRequest = "{\n"
                        + "\"token\" : \""
                        + connToken
                        + "\","
                        + "\"dbName\": \""
                        + dbName
                        + "\",\n" + "\"cmd\" : \"PUT\",\n"
                        + "\"rel\" : \""
                        + relName + "\","
                        + "\"jsonStr\": \n"
                        + jsonObj
                        + "\n"
                        + "}";
                return putRequest;
            }
            function executeCommand(reqString, dbBaseUrl, apiEndPointUrl) {
                var url = dbBaseUrl + apiEndPointUrl;
                var jsonObj;
                $.post(url, reqString, function (result) {
                    jsonObj = JSON.parse(result);
                }).fail(function (result) {
                    var dataJsonObj = result.responseText;
                    jsonObj = JSON.parse(dataJsonObj);
                });
                return jsonObj;
            }
            function resetForm() {
                $("#empId").val("")
                $("#empName").val("");
                $("#empEmail").val("");
                $("#empId").focus();
            }

            function saveEmployee()
            {
                var jsonStr = validateAndGetFormData();
                if (jsonStr === "") {
                    return;
                }
                var putReqStr = createPUTRequest("90935796|-31948838699886563|90934728",
                        jsonStr, "SAMPLE", "EMP-REL");
                alert(putReqStr);
                jQuery.ajaxSetup({async: false});
                var resultObj = executeCommand(putReqStr,
                        "http://api.login2explore.com:5577", "/api/iml");
                alert(JSON.stringify(resultObj));
                jQuery.ajaxSetup({async: true});
                resetForm();
            }
        </script>
    </body>
</html>

<img src="https://user-images.githubusercontent.com/66720092/110651464-78d85400-81e1-11eb-95e4-c8a7e1182e96.jpg" width="1000">

