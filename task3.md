By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad**
![WhatsApp Image 2024-02-27 at 11 21 19 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/c8ee703b-e538-4c6f-948c-c8a27818a16a)
**Step 2: Writing the C code in the leafpad editor using the following command

leafpad sum1ton.c&
![WhatsApp Image 2024-02-27 at 11 21 49 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/8087ec07-d30f-4401-a920-11d97c1cb388)
Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c
![WhatsApp Image 2024-02-27 at 11 22 50 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/007f4de7-8540-425c-adb2-e86f1dbc5578)
Step 5: Check the output by using the command

./a.out
![WhatsApp Image 2024-02-27 at 11 25 08 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/e134b545-260d-4648-a31d-4f75db9a0f3b)
The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c
![WhatsApp Image 2024-02-27 at 11 26 12 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/9c9924b3-20b5-4f67-8caa-18009e953c66)
Step 2: Compile the code in riscv using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![WhatsApp Image 2024-02-27 at 11 28 28 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/b55632ab-28a5-4ca8-8e20-ba36ebdb89b5)
Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command

ls -ltr sum1ton.c
![WhatsApp Image 2024-02-27 at 11 29 35 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/10da3e78-f6d4-41f2-9dc6-985675522ea5)
![WhatsApp Image 2024-02-27 at 11 40 26 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/9df96ae2-5558-451d-a76d-5f9c59f87428)
Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution
![WhatsApp Image 2024-02-27 at 11 43 05 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/23aeaaac-adfa-4b8f-9049-fc5da3289b38)
![WhatsApp Image 2024-02-27 at 11 43 05 AM (1)](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/15367787-10c2-4162-bdc2-2f0b0ece8c52)
Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![WhatsApp Image 2024-02-27 at 11 43 05 AM (2)](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/8ee47ee9-9d35-43ef-ba9b-29f0d1ff115a)
![WhatsApp Image 2024-02-27 at 11 43 06 AM](https://github.com/Suraiya2003/SURAIYA-NAAZ-8/assets/160725650/87d763c4-1c1e-441e-97b1-0f00a97f0e4b)








