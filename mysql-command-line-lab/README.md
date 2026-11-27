## Configuring MySQL in Windows Environment Variables

The following steps allow you to access MySQL directly from PowerShell or Command Prompt without manually navigating to the installation folder each time.

### Step-by-Step Instructions

1. Navigate to the Windows search bar on the taskbar and search for **View advanced system settings**.

2. Click **View advanced system settings** to open the System Properties window.

3. At the bottom of the window, click **Environment Variables**.

4. Under the **User variables** section, locate and select **Path** to highlight it.

5. Click the **Edit** button next to the **New** button.

6. The **Edit environment variable** window will appear.

7. Click **New** to create a new entry.

8. A text box will appear underneath the last entry. Enter the following MySQL installation path:

   `C:\Program Files\MySQL\MySQL Server 8.0\bin`

9. Once the path has been entered, click **OK** on both windows, then close the System Properties window.

10. Open a new PowerShell or Command Prompt window to verify that the configuration was successful.

### Verifying the Configuration

Enter the following command to verify that MySQL is accessible:

`mysql --version`

To connect to the local MySQL server, enter:

`mysql -u root -p`

Enter your MySQL root password when prompted.

### Final Result

MySQL can now be accessed directly from PowerShell or Command Prompt without manually navigating to its installation directory. This configuration simplifies database access and improves workflow efficiency.
