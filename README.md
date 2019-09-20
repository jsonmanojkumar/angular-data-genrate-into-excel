# install

npm install file-saver --save  
npm install xlsx --save 
npm install bootstrap  

# imports
# Open the excel-services.service.ts file and add the following code into it.

import { Injectable } from '@angular/core';  
import * as FileSaver from 'file-saver';  
import * as XLSX from 'xlsx';  
const EXCEL_TYPE = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet;charset=UTF-8';  
const EXCEL_EXTENSION = '.xlsx';  

# Here is the code for app.component.ts.
import { Component, OnInit } from '@angular/core';  
import { ExcelServicesService } from './services/excel-services.service';  
import { HttpClient } from '@angular/common/http';  
import { Observable } from 'rxjs';  

# Here is the code for app.module.ts.
import { BrowserModule } from '@angular/platform-browser';    
import { NgModule } from '@angular/core';    
import { HttpClientModule } from '@angular/common/http';    
import { AppRoutingModule } from './app-routing.module';    
import { AppComponent } from './app.component'; 


# genrate service
ng g service ./services/excel-services 

# AngularDataGenrateExcel

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.5.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
