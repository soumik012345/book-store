# POS – “Point of Sale” (FrontEnd)
-----------------------------------------------------------------

## 1. [Documentation](https://github.com/togetherGithub/Point-Of-Sale)

## 2. Automation Source Code
* 2.1 [Backend](https://github.com/togetherGithub/Point-Of-Sale/tree/main/rest-service)
* 2.1 [Frontend](https://github.com/togetherGithub/Point-Of-Sale/tree/main/web-client-v2)

## Prerequisites

### Install Node JS
Refer to https://nodejs.org/en/ to install nodejs

## Development server

Run `npm start` for a dev server. Navigate to `http://localhost:3000/`. The app will automatically reload if you change any of the source files.

Or

### How to start

**Note** that this seed project requires **node.

In order to start the project use:

```bash
# install the project's dependencies
$ npm install
# watches your files and uses livereload by default run `npm start` for a dev server. Navigate to `http://localhost:3000/`. The app will automatically reload if you change any of the source files.
$ npm start
# prod build, will output the production application in `dist`
# the produced code can be deployed (rsynced) to a remote server
$ npm run build
```

## Application design

#### Components

1. **Customers** Component : This Component displays a list of customers. This Component gets the data from a json file in assets folder

2. **CustomerDetails** Component : This Component Displays the details of the selected customer. This Component gets its data from a json file in assets folder as well. This Component is the Child Component of *Customers* Component

#### HTTP client

**axios** library is used to make HTTP Calls

## Resources

**create-react-app** : The following link has all the commands that can be used with create-react-app
https://github.com/facebook/create-react-app

**ReactJS** : Refer to https://reactjs.org/ to understand the concepts of ReactJS

**React Bootstrap** : Refer to https://react-bootstrap.github.io/getting-started/introduction/ to understand how to use React Bootstrap


## Folder Structure

Within the download will find the following directories and files, logically grouping common assets and providing both compiled and minified variations and see something like this:

```
web-client-v2
├
├──── .github      
├──── node_modules 
├──── public  
├──── src 
├── .browserslistrc 
├── .editorconfig 
├── .env   
├── .eslintrc.js 
├── .gitattributes 
├── .gitignore 
├── .prettierignore 
├── .prettierrc.js 
├── CHANGELOG.md 
├── jest.config.js
├── jsconfig.json 
├── LICENSE  
├── migration.md  
├── package.json
├── package-lock.json
└── README.md 

```

```
7.	src
8.	│   App.css
9.	│   App.js
10.	│   App.test.js
11.	│   index.js
12.	│   routes.js
13.	│   serviceWorker.js
14.	│   setupTests.js
15.	│   store.js
16.	│   tree.txt
17.	│   _nav.js
18.	│
19.	├───assets
20.	│   ├───brand
21.	│   │       logo-negative.js
22.	│   │       logo.js
23.	│   │       sygnet.js
24.	│   │
25.	│   └───images
26.	│       │   angular.jpg
27.	│       │   react.jpg
28.	│       │   vue.jpg
29.	│       │
30.	│       ├───avatars
31.	│       │       1.jpg
32.	│       │       2.jpg
33.	│       │       3.jpg
34.	│       │       4.jpg
35.	│       │       5.jpg
36.	│       │       6.jpg
37.	│       │       7.jpg
38.	│       │       8.jpg
39.	│       │       9.jpg
40.	│       │
41.	│       └───CreditCard
42.	│               creditCard.jpg
43.	│
44.	├───components
45.	│   │   AppBreadcrumb.js
46.	│   │   AppContent.js
47.	│   │   AppFooter.js
48.	│   │   AppHeader.js
49.	│   │   AppSidebar.js
50.	│   │   AppSidebarNav.js
51.	│   │   DocsCallout.js
52.	│   │   DocsExample.js
53.	│   │   DocsLink.js
54.	│   │   index.js
55.	│   │
56.	│   ├───handleErrors
57.	│   │       HandleClientSideError.js
58.	│   │       HandleServerSideError.js
59.	│   │
60.	│   ├───header
61.	│   │       AppHeaderDropdown.js
62.	│   │       index.js
63.	│   │
64.	│   ├───invoicer
65.	│   │       ClientDetails.js
66.	│   │       Dates.js
67.	│   │       Footer.js
68.	│   │       Header.js
69.	│   │       Invoice.js
70.	│   │       Notes.js
71.	│   │       Table.js
72.	│   │       UserDetails.js
73.	│   │
74.	│   └───recursionTree
75.	│           Tree.css
76.	│           Tree.js
77.	│           TreeList.js
78.	│
79.	├───constants
80.	│       appConstant.js
81.	│
82.	├───layout
83.	│       DefaultLayout.js
84.	│
85.	├───scss
86.	│       style.scss
87.	│       _custom.scss
88.	│       _example.scss
89.	│       _layout.scss
90.	│       _variables.scss
91.	│
92.	└───views
93.	    │   tree.txt
94.	    │
95.	    ├───autoSuggest
96.	    │       AutoSuggest.css
97.	    │       AutoSuggest.js
98.	    │
99.	    ├───category
100.	    │   ├───addCategory
101.	    │   │       AddCategrory.js
102.	    │   │       DeleteCategory.js
103.	    │   │       EditCategory.js
104.	    │   │
105.	    │   └───categoryList
106.	    │           CategoryList.js
107.	    │
108.	    ├───customer
109.	    │   ├───components
110.	    │   │       AddCustomer.js
111.	    │   │       DeleteCustomer.js
112.	    │   │       EditCustomer.js
113.	    │   │
114.	    │   └───customerList
115.	    │           CustomerInformation.js
116.	    │           CustomerList.js
117.	    │
118.	    ├───dashboard
119.	    │       Dashboard.js
120.	    │
121.	    ├───pages
122.	    │   ├───login
123.	    │   │       Login.js
124.	    │   │
125.	    │   ├───page404
126.	    │   │       Page404.js
127.	    │   │
128.	    │   ├───page500
129.	    │   │       Page500.js
130.	    │   │
131.	    │   └───register
132.	    │           Register.js
133.	    │
134.	    ├───paginationArea
│       PaginationArea.js
136.	    │
137.	    ├───product
138.	    │   ├───components
139.	    │   │       AddProduct.js
140.	    │   │       DeleteProduct.js
141.	    │   │       EditProduct.js
142.	    │   │
143.	    │   └───productList
144.	    │           ProductList.js
145.	    │
146.	    ├───purchase
147.	    │   ├───addPurchase
148.	    │   │       AddPurchase.js
149.	    │   │       HandleBarcodeFound.js
150.	    │   │       HandleNoBarcode.js
151.	    │   │       HandleSummary.css
152.	    │   │       HandleSummary.js
153.	    │   │       ProductNameOverlay.js
154.	    │   │       SearchProductName.js
155.	    │   │       WarningPopup.js
156.	    │   │
157.	    │   └───purchaseList
158.	    │           PurchaseList.js
159.	    │
160.	    ├───Sale
161.	    │   ├───addSale
162.	    │   │       AddSale.js
163.	    │   │       HandleBarcodeFound copy.js
164.	    │   │       HandleNoBarcode.js
165.	    │   │       HandleSummary.js
166.	    │   │       ProductNameOverlay.js
167.	    │   │       SearchProductName.js
168.	    │   │       WarningPopup.js
169.	    │   │
170.	    │   └───saleList
171.	    │           SaleList.js
172.	    │
173.	    ├───stock
174.	    │       Stock.js
175.	    │
176.	    ├───Transaction Settlement
177.	    │   │   TransactionMethods.js
178.	    │   │   
179.	    │   ├───transactionMethods
180.	    │   │       AddTransaction.js
181.	    │   │       DeleteTransaction.js
182.	    │   │       EditTransaction.js
183.	    │   │
184.	    │   └───transactionSettlement
185.	    │       │   TransactionSettlement.js
186.	    │       │
187.	    │       └───settlementComponent
188.	    │               TransactionDetails.js
189.	    │               TransactionSettle.js
190.	    │
191.	    ├───unit
192.	    │   ├───components
193.	    │   │       AddUnit.js
194.	    │   │       DeleteUnit.js
195.	    │   │       EditUnit.js
196.	    │   │
197.	    │   └───unitList
198.	    │           UnitList.js
199.	    │
200.	    └───widgets
201.	            Widgets.js
202.	            WidgetsBrand.js
203.	            WidgetsDropdown.js


