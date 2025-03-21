# React Developer Test

The task is to create a React JS application, using only [Typescript](https://www.typescriptlang.org/), [React Router](https://reacttraining.com/react-router/web/guides/quick-start) and [React Context](https://reactjs.org/docs/context.html), that will show list of products and allows users to add products to the shopping basket.

Keep away from unnecessary dependecies, keep it simple.

## Getting started

1. Start client using `yarn serve:client`
   it will start on [localhost:3000](http://localhost:3000)
2. Start server using `yarn serve:server`
   it will start on [localhost:3001](http://localhost:3001)

## API Documentation

1. `http://localhost:3001/api/products/ (GET)` - get list on products.

   ```ts
   interface Product {
     name: string;
     category: Category;
     price: number;
   }
   ```

2. `http://localhost:3001/api/product/categories/ (GET)` - get list of categories.
   ```ts
   interface Category {
     id: string;
     name: string;
   }
   ```

## Todo:

<ol>
  <li>Create page with list of products.
    <ul>
      <li>Fetch list of products.</li>
      <li>Show all the products in a table.</li>
      <li>Add possibility to add in cart.</li>
      <li>Add possibility to remove from cart directly in list of products table.</li>
    </ul>
  </li>

  <li>Add posibility to filter products by <b>categories</b> and sort price by <b>desc</b> or <b>asc</b>.</li>

  <li>Create page with list of added products.
    <ul>
      <li>Show all the added products in a table.</li>
      <li>Add possibility to change quantity of added products.</li>
      <li>Add possibility to remove added product.</li>
       <li>Show total price for all added products</li>
    </ul>
  </li>
</ol>

## Examples:

List of products example:
| Category ^ | Name | Price ^ | Actions |
|------------------------------|:---------|:--------|:--------------:|
| Vegetables and legumes/beans | Broccoli | \$0.25 | (-) Select (+) |

List of added products example:
| Category | Name | Quantity | Price | Actions |
|------------------------------|:---------|:---------|:------|:--------------:|
| Vegetables and legumes/beans | Broccoli | 2 | \$0.50 | (-) Remove (+) |
