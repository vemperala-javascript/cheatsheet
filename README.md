


# safe navigation operator
# products?.length==0   
above statement is equal to  
if(products is null\undefined) || (products.length ==0)     

https://angular.io/guide/template-syntax#safe-navigation-operator  


# routerLink
routerLink="/products/{{ product.id }}"     

# ActivateRoute
route:  ActivateRoute

# path
route:  ActivateRoute
const route: Router = [ {path: 'product/:id', component: ProductComponent} ]

# string to number
// get the id from param string and convert the string to a number using the "+" symbol  
const productid: number = +this.route.snapshot.paramMap.get('id');

# observable subscribe
this.productservice.getproduct().subscribe(   
 {  data => this.product = data;})
 
 # template string
 `{this.value}`

# onNgInit
onNgInit(): void {  
this.route.paramMap.subscribe(()=> {  
somemethod();  
})  
}

# observable
 getProduct(theProductId: number): Observable<Product> {  

    // need to build URL based on product id  
    const productUrl = `${this.baseUrl}/${theProductId}`;  

    return this.httpClient.get<Product>(productUrl);   
  }

# angular language serivce
intall plugin in vss code.  
view -> extennions -> angular language service   
this. extension helps tocompile. the agular code and show any errors at the compile time  

# ng booststrap 
this is used for pagination.  

ng add @angular/localize  
npm install @ng-bootstrap/ng-bootstrap    

this command is to fix some warnings when you do an npm install  
npm audit fix  
and then in Ngmodule file import the NgbModule and also add ngbModule in imports array  

# Subject
Subject is a sub class of Observable   
it is used to publish the events to subscribers  
price : Subject<number> = new Subject<number>()  
 andd now to publish the upddated value of price.  
 price.next(10);  
 
# only show 2 digits after the decimal eg 148.98
price.toFixed(2)  

# Arrays.find()
cartitems.find(tempcartitem => tempcartitem.id === thecartitem.id);  
the method returns the first element in an array that passes the test.  
