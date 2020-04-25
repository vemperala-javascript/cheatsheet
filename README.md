


# safe navigation operator
# products?.length==0   
above statement is equal to
if(products is null\undefined) || (products.length ==0) 

https://angular.io/guide/template-syntax#safe-navigation-operator


# routerLink
routerLink="/products/{{ product.id }}" 


# path
const router: Router = [ {path: 'product/:id', component: ProductComponent} ]

# string to number
// get the id from param string and convert the string to a number using the "+" symbol
const productid: number = +this.route.snapshot.paramMap.get('id');

# observable subscribe
this.productservice.getproduct().subscribe(
 {  data => this.product = data;})
 
 # template string
 `{this.value}`
