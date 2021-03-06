# VS Code Cypress Snippets

This extension contains [Cypress](https://cypress.io/) code snippets used by [Andrew Smith](https://andrew.codes). Work in Progress.

## Installation

In order to install an extension you need to launch the Command Palette (Ctrl + Shift + P or Cmd + Shift + P) and type Extensions.
There you have either the option to show the already installed snippets or install new ones.

## Supported Languages (file extensions)

- JavaScript (.js)
- TypeScript (.ts)
- JavaScript React (.jsx)
- TypeScript React (.tsx)

## Snippets

### visit (`cyv`)
```javascript
cy.visit('$1');$0
```
### get element(s) (`cyge`)
```javascript
cy.get('$1')${0:;}
```
### get elements (alternative) (`cyget`)
```javascript
cy.get('$1')${0:;}
```
### get alias (`cyga`)
```javascript
cy.get('@$1')${0:;}
```
### get and alias element(s) (`cygaa`)
```javascript
cy.get('$1').as('$2')${0:;}
```
### find (`cyf`)
```javascript
find('$1')${0:;}
```
### first (`cy1`)
```javascript
first()${0:;}
```
### last (`cyl`)
```javascript
last()${0:;}
```
### at index (`cyeq`)
```javascript
eq($1)${0:;}
```
### type (`cyt`)
```javascript
type('$1')${0:;}
```
### contains (`cycon`)
```javascript
contains(${2:'$3', }'$1')${0:;}
```
### click (`cyc`)
```javascript

click()${0:;}
```
### server (`cyserver`)
```javascript
cy.server();$0
```
### route (`cyroute`)
```javascript
cy.route(${2:'$3', }$1).as('${4}');$0
```
### wait (`cyw`)
```javascript
cy.wait(${1:'@${2}'});$0
```
### viewport (`cyvp`)
```javascript
cy.viewport($1, $2);$0
```
### request (`cyreq`)
```javascript
cy.request({
	method: '$1',
	url: '$2',
	headers: { 'Accept-Language': 'en-us', },
});$0
```
### add command (`cyadd`)
```javascript
Cypress.Commands.add('$1', ${3: { previous: '$4' \} , }$2);$0
```
