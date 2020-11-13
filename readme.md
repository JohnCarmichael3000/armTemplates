Windows 10 Desktop VM Deploy with this script. Run script or activate via clicking button below.

Windows 10 Pro with:
- Creates compute extension to run Powershell script after VM creation. PS script installs Chocolatey package manager.
- Uses Spot pricing on Azure meaning machine is only active when space is available to save cost. You can go for a lower per hour spot price, but for $0.10/hr USD you can have a machine that generally won't be ejected. https://azure.microsoft.com/en-us/pricing/spot/ "With Azure Spot Virtual Machines (Spot VMs), you can access unused Azure compute capacity at deep discounts—up to 90 percent compared to pay-as-you-go prices.* You pay up to the maximum price that you optionally agree to in advance."
- Non-standard range IP, useful as the default Azure IP/IP Range 10.0.0.x can be used by other products and cause conflicts.
- Automatic shutdown: even though spot pricing is quite inexpensive, automatic shutdown prevents your VM from running continuously if you get distracted by something else.
- Chocolatey software Package manager installed. Why install software manually when you can script it? https://chocolatey.org/
- Latest Google Chrome browser and Microsoft Visual Studio Code auto installed with Chocolatey.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FJohnCarmichael3000%2FarmTemplates%2Fmain%2Fwindows10_development_vm.json)



