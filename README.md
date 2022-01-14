Tested with Magento v2.3.x till Magento 2.4.3-p1

# Magento2.3 or greater version After installing getting blank screen or getting Exception
1 exception(s): Exception #0 (Magento\Framework\Exception\ValidatorException): Invalid template file: '...vendor/magento/module-theme/view/frontend/templates/page/js/require_js.phtml' in module: '' block's name: 'require.js'

# In developer Mode - with Exception 
![Error Screenshot](storefront.png)

![Error Screenshot](admin.png)


# In default Mode - blank screen or not loading all data
![Error Screenshot](default-mode-storefront.png)

![Error Screenshot](default-mode-admin.png)

# To fix apply shared patch

`git apply`  [kanhaiya5590-M2.3-black-gray-screen-issue.patch](kanhaiya5590-M2.3-black-gray-screen-issue.patch)

 ***Note: considering we downloaded the patch file on root of the project directory or updated path in command accordingly, when executing command***
 
 
 # To revert the applied patch
 `git apply -R` [kanhaiya5590-M2.3-black-gray-screen-issue.patch](kanhaiya5590-M2.3-black-gray-screen-issue.patch)
