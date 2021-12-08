# uts-abbrorsholakhudin
proses data warehouse menggunakan mariadb dari  database sumber (classicmodels) ke data base tampung (utsabbror)
1. pertama buat table dimensi untuk menentukan table mana yang ajan dipilih, disini saya menggunakan table, customer,product,orders
2. buat transformasi  ETL(ekstrak Transform Load) menggunakan pentaho data-integration bernama dim_customer.ktr,dim_product.ktr,dim_order.ktr
3. jalankan transformasi hingga dapat masuk ke table dimensi yang kita buat
4. buat table fakta untuk sebagai summary/ gabungan dari 3 table dimensi tsb yang berisi id dari setiap table dan ammount sebagai nilai
5. selesai , table fakta terdapat suatu insight yaitu customer x membeli produk x dengan nomor order x 
