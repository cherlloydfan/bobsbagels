# bobsbagels
As a member of the public
So I can order a bagel when I want to
I'd like to add an item to my basket

Objects:Basket, Item,   
Properties: Items @Array,Item name @String, 
Messages:AddToBasket(@Item), OrderItem(@Item),          
Outputs:Item added to basket(@String), Item ordered(@String) 

As a member of the public,
So that I can change my order
I'd like to remove an item from my basket

Objects:item, basket    
Properties: item name@string, item@array 
Messages: removeFromBasket(), updateBasket()         
Outputs: item removed from basket, basket updated

# Part 2
As a member of the public,
So that I can not overfill my small bagel basket
I'd like to know when my basket is full when I try adding an item beyond my basket capacity.

objects: bagel basket, customer
properties:basket@integer,customerID@integer
Messages:checkCapacity(),getCustomer()
Output:tell you the capacity, checks which customers basket it is

As a Bob's Bagels manager,
So that I can record more sales
I’d like to create baskets with larger capacity when I need to.

objects: basket,Manager
properties:basketCapacity@integer, ManagerName@String,
Messages:editBasket(), recordSales()
Output:updates basket capacity,manger get sales data

As a member of the public
So that I can maintain my sanity
I'd like to know if I try to remove an item that doesn't exist in my basket. In the same way, I want to know if I try to add an item with the same ID already in my basket.

objects: item, basket
properties:itemName@String, basketID@Integer ItemID@Integer
Messages:deleteItem(), addItem(),checkBasket()
Output:says if it doesn't exist,notifies if that item is already in the basket

# Part 3
As a member of the public,
So that I can know how much my bagels are,
I’d like to see the price of each item before I add it to my basket.

objects: item
properties:itemPrice@Currency   ItemName@String
Messages:getItemPrice(),getItemName()
Output:gives the price

As a member of the public,
So that I can prepare to pay
When I go to checkout I'd like to know the total sum of the bagels in my basket

objects: items
properties:itemQuantity@Integer , ItemPrice@Currency, ItemName@String
Messages:checkout()
Output:gives the cost of items