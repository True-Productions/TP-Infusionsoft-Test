# True Productions Infusionsoft Test

## Build a simple page and API that takes data from a POST request and inserts it into a CRM

Thank you for your interest in employment at True Productions! We want you to demonstrate your proficiency in PHP & JavaScript by writing an application that mirrors many of the tasks that you will be requested to perform for True Productions. Namely, you are to write a basic end-to-end application that:

* Presents a user with a web page that contains a text input box and button
* Allows the user to submit data to an API
* and Passes the submitted data to Infusionsoft (a CRM) and saves it into a contact's contact record.

Below are the basic specifications of the project:

1. Design a PHP class that creates an Infusionsoft SDK object, stores it and allows any method to use this object.
2. Design a method in this class that takes data and stores it into a contact record's custom field.
3. Design a REST end point that received POST data and does the following:
   * Validates the POSTed data  
   * Creates an instance of above class
   * Uses the class to send the data to Infusionsoft
   * Returns data in JSON format that indicates success or failure
4. Design a web page that sends an AJAX POST request to a REST end point (Doesn't matter if you use jQuery, Axios,  Fetch API, raw XHR, Axios, etc. It simply needs to work).
5. On response from the AJAX POST, display a success or error message.

Below is what is provided:

* index.html
  * This page includes a basic input field and button, plus an empty div where messages should reside. Please use this barebones template for all customer facing HTML and JavaScript.

* api/Infusionsoft
  * The Infusionsoft SDK (iSDK). The SDK shouldn't be modified, except for inclusion of the Infusionsoft App title and encrypted key.

* api/classes/infusionsoft_test_class.php
    * This is the class that you need to extend to handle all usage of the Infusionsoft SDK. This class must create and maintain an Infusionsoft SDK object and utilize a method to send data to Infusionsoft via the object.

* api/test.php
  * This file is a barebones php script that simply requires the class file listed above. Create a REST API that accepts POSTs, uses the class you designed above to send data to Infusionsoft based upon user input.

Documentation:

We recommend you use [Infuionsoft's Developer documentation (https://developer.infusionsoft.com/docs/xml-rpc/)](https://developer.infusionsoft.com/docs/xml-rpc/) to learn how to use the SDK. All code examples are listed under PHP iSDK. We also recommend that you read the readme within the Infusionsoft folder.

You will be provided the following information on the onset of the test:

* The Application Name
* The API Key
* The Contact ID

The application name and API key are to be placed into the file at /api/infusionsoft/conn.cfg.php to connect correctly and the Contact ID is the ID where data will be stored.

Good luck!