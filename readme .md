# Project Title
Error Handling and its methods

This is the Module 1 assesment of Eth+AVAX proof course . This is a solidity program for implementing the error handling concept and its method which consist of require() revert() and assert() methods  .

## Description

This is a program which is created in solidity for using the concept of errror handling and implementing its methods which uses the basic concept of solidity like working in remix ethereum and writing a code in .sol file which contains the intermediate knowledge like error handlng and its methods . This program show the use of error handling method and also its implementation.

## Getting Started


### Executing program

To run this program , i am using Remix , an Solidity IDE.
->To start go to Remix IDE and start coding 
->add a solidity file i named it as multiplication.sol
->include the licence (SPDX) 
->use the latest solidity compiler by including the pragma which will compiler the code using that solidity compiler
->make a contract named Multiplyusingrra 
->under that contract create a function named multiplication which take two parameters of unsigned interger (uint256) type _a and _b.
->write require method with some condition  which ensures that _a and _b should always be grater than 0. if it is 0 then an error message will revert. 
->write revert method with some condition which ensures that mutiplication should always be greater than 100 . if it is not than error messsage will revert.
->write assert methhod which will only consist only one statement which ensure _b should be greater than _a , if not then transaction is revert.
->click on compile (compilemultiplication.sol)
->go to deploy and deploy it.

code blocks for commands
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract Multiplyusingrra {
   
    function multiplication(uint256 _a, uint256 _b) external pure returns (uint256) {

        // require statement
        require(_a>0 && _b>0 , "input must be greater than 0 for multiplication");

        // assert statement
        assert(_b>_a);

        //Perform Multiplication
        uint256 multiply=_a * _b;

        // revert statement
        if (multiply > 100) {
            revert(" Multiplication overflow");
        }

        return multiply;
    }
}

## Help

Change the compiler solidity version if error occur , then change by going to compiler solidity menu present on left side of the compiler and change the compiler version.

## Authors

->Amrita Kumari
->https://www.linkedin.com/in/amrita-kumari-753319232/

## License

This project is licensed under the MIT License - see the licence file for details.
