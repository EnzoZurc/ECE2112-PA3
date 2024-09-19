# ECE2112-PA3
Name: Cruz, Christian Enzo B. </br>
Section: 2ECE-D </br></br>
## Experiment 3 - PANDAS
Before continuing to the problems we have to access the pandas library by inputing the code function below.</br>
![image](https://github.com/user-attachments/assets/e47bbe04-b932-4fbd-93b4-6f9e0ef1c4d9)

#### Problem 1
##### a. Load the corresponding .csv file into a data frame named cars using pandas. </br>
After downloading the given cars file, to load it on our notebook we have to use the pandas code read_csv so we could view the given csv file.</br>
![image](https://github.com/user-attachments/assets/db9d6aa7-5300-4f82-8246-d0e94759d956) </br>

Running this code would make us able to observe the given file shown on the image below </br>
![image](https://github.com/user-attachments/assets/7e0baf87-330c-4459-85d3-ad7b814eecfb)</br></br>

##### b. Display the first five and last five rows of the resulting cars.</br>
After successfully loading the csv file, we now have to load the first 5 rows and we can do that by using the pandas code heads(5) shown on the image below.</br>
![image](https://github.com/user-attachments/assets/800235c7-f718-4dc3-96db-ee73a6af4bc9)</br>

And now to load the last 5 rows we will be using the pandas code tail(5) shown on the image below.</br>
![image](https://github.com/user-attachments/assets/73b552b3-d1d8-469f-a0cf-12b97c389c05)</br></br>

#### Problem 2
By using the dataframe cars  in problem 1, extract the following information using subsetting, slicing and
indexing operations.</br>

##### a. Display the first five rows with odd-numbered columns (columns 1, 3, 5, 7…) of cars.
To display the first odd 5 columns we have to access the rows and columns. We first have to find the odd columns.</br>
By using the code function below I was able to find it. The iloc function was used to access the rows and columns of the data frame.</br>
![image](https://github.com/user-attachments/assets/5183fff4-af7a-4251-b1e5-c8ed654557ab)</br>
Afterward I used the function head(5) to display the first 5 rows of the odd columns shown on the image below.</br>
![image](https://github.com/user-attachments/assets/4c77193a-722d-459f-a9a5-75af51d97edb) </br></br>

##### b. Display the row that contains the ‘Model’ of ‘Mazda RX4’.
Now to the specifics we have to find the row that contains the given car model. By using cars['Model'] == 'Mazda RX4': This creates a boolean Series that checks each value in the 'Model' column to see if it matches the string 'Mazda RX4'. The result is True for rows where the model is 'Mazda RX4' and False otherwise. This can be shown on the image below.</br>
![image](https://github.com/user-attachments/assets/c1db0e3f-10e9-4a80-a932-3771ada4634e)</br></br>

##### c. How many cylinders (‘cyl’) does the car model ‘Camaro Z28’ have?
Now we are asked to find how many cyl does the given car model have. Similar to the previous requirement we have to make a boolean series that checks the car model, but this time we have to also find how much is its cylinders and this can be achieved by using the function "cars.loc[cars['Model'] == 'Camaro Z28', ['cyl']]", by adding the ', ['cyl']' at the end after checking the model, it would make the function check its cyl column. This can be shown on the image below.</br>
![image](https://github.com/user-attachments/assets/420103f2-4fcc-49fc-b825-1ea30aa8513f)</br></br>

##### d. Determine how many cylinders (‘cyl’) and what gear type (‘gear’) do the car models ‘Mazda RX4 Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ have.
Similar to the previous requirement we have to find how many cyl the car models have but this time with the gear. Using a similar function "cars.loc[cars['Model'] == 'Mazda RX4 Wag', ['cyl','gear']]" by adding the gear at the end the function would also check the gear column of the given car model. Since there are 3 car models given this would be repeated 3 times we just have to change what model is being checked. This can be shown on the image below. </br>
![image](https://github.com/user-attachments/assets/c3fdfa4c-28fb-4687-b377-7f32e4a65791)</br>
![image](https://github.com/user-attachments/assets/a23c386b-0d04-4c31-b5bb-2c75bbe1cdb8)</br>
![image](https://github.com/user-attachments/assets/2c0ad33f-3ef5-401d-9e76-a81fe76ebb01)


