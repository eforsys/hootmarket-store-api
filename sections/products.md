Products
========

The products API allows access all products enabled to be sold.

Get products
------------
* `GET /products.json` Return all products enabled to be sold.

**Params**

* `limit=#{quantity}` limits the number of products returned. The default quantity is 20, maximun 100 and minimun 1.
* `page=#{page_number}` specifies the page.
* `order=(#{field} asc | #{field} desc)` specifies the order of products.

**Response**

``` json
{
  products: [
    {
      id: id,
      name: name
    },
  ],
  pagination: {
  }
}
```

Get product
-----------
* `GET /product/#{code}.json`
