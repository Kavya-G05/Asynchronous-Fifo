# TESTBENCH  
The data **WIDTH** is chosen as **4** and FIFO **DEPTH** is chosen as **8**. Random data is generated and given to the `wdata` port. The `rst_n` signal is used to reset the **read & write pointers** and assert the **empty** flag.   

# OUTPUTS 
- A **three-cycle delay** is observed in de-asserting the **empty** flag. This is because the write-pointer update is reflected in the **read clock domain** only after three cycles.  
- Data written into the **write clock domain** is successfully synchronized and read in the **read clock domain**.

  ![image](https://github.com/user-attachments/assets/04d26730-6db6-414d-bcc7-26f8c8da4cdf)

