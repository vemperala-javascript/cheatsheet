


# safe navigation operator
# products?.length==0   

above statement is equal to

if(products is null\undefined) || (products.length ==0) 


https://angular.io/guide/template-syntax#safe-navigation-operator


# routerLink
<a routerLink="/products/{{ product.id }}" />

# path

const router: Router = [
{path: 'product/:id', component: ProductComponent}
]
