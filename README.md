backend\models\Item.js
la ----
 
	//ithu serialNumber add panra code
    serialNumber: {
      type: String,
      required: [true, "Serial Number is required"],
      trim: true,
      unique: true,
    },
	//ithoda mudinshu
  

frontend\src\components\ItemForm.jsx

la ----


 
      name: "",
      category: "",
      price: "",
      description: "",
      imageUrl: "",
      serialNumber: "",                       <-----ithula add pannanum
  

ithe fille la kila ithu varum 


      <label>Serial Number</label>
      <input name="serialNumber" value={formData.serialNumber} onChange={handleChange} required />


frontend/src/components/ItemCard.jsx

la ---
       
	  <h3>{item.name}</h3>
      <p><strong>Serial Number:</strong> {item.serialNumber}</p>                     <----itha add pannu
      <p><strong>Category:</strong> {item.category}</p>
      <p><strong>Price:</strong> ${item.price}</p>
      <p>{item.description}</p>
