# IMS_Yesh
 The Inventory managment system project
->IMS works as follows. Intially 37 values are appended into a Json file named Dataset_mod_6.json. This can be done by directly appending the values as key value pairs or by taking individual inputs. The json dataset has attributes such as Name of the item, Type of the item, cost, suitability etc.

->This dataset is more like the attributes that every E-Commerce product has on websites like Amazon, Flipkart, E-Bay etc.

->For simplicity, each product initially has 80 items in the inventory.

->Updates to the existing inventory can be made by reading the file, Converting json back to a dictonary and then modifying desired values. The process ends with converting the modified dictonary back to json and writing the updated data to the file.

->Finally, we have the user module which takes inputs form user as the product and product quantity. But, the user generally doesn't stop with 1 product. To accomplish this, an infinite while loop prompts the user until he/she is satisfied with the cart.

->Next we need to retrieve the item prices from the dataset and calculate price based on number of units asked. The previously converted dictionary "convnext" is handy in this process. A loop is used to find the desired items in the dictionary and thus important values ID, Product name and price are retrieved and appended as a list to a result list.

->Such lists are traversed to generate a bill and that is the final module. In the mean time, the inventory should also be updated in-terms of number of items available. For instance products with IDs  11652255,11652267 are have their quantities updated to 78 each which is clearly seen in the JSON file.

->After updating the quantity attribute, the latest Dictionary is converted back to json and written back to the json file.
