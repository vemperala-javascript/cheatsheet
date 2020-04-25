


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
this. extension helps tocompile. the agular code and how any errors at the compile time
