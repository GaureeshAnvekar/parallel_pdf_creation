# Parallel PDF Creation




A tool for Data Analysts/Business Analysts. With this, it first creates a pdf template based on the columns of the dataframe. Then it fills this template pdf creating multiple pdfs representing each row of the dataframe. This can be done for multiple dataframes as well. The task is parallelized using multithreading.
https://pypi.org/project/parallel-pdf-creation/


## Installation


```sh
pip install parallel_pdf_creation

```
## Initial Setup
1. Initial setup is required before the package runs successfully. (pdftk-server)
1. For Windows, install pdftk-server from, 
https://www.pdflabs.com/tools/pdftk-server/
If “pdftk” is not detected in the terminal, you need to setup the environment variable PATH.
This is a good link that describes the steps for Windows 7 onwards, to setup PATH variable.
https://ourcodeworld.com/articles/read/240/how-to-edit-and-add-environment-variables-in-windows-for-easy-command-line-access 
1. For macOS, get the latest version of “pdftk-server”, with this link, and install it,
https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit/pdftk_server-2.02-mac_osx-10.11-setup.pkg
It may say permission not granted. Go to “System preference”, “security”, then unlock the access for the above installation.



After installation, use it directly in the jupyter notebook as,
```
import parallel_pdf_creation as ppc

ppc.begin({"name_of_df1": df1, "name_of_df2": df2, .....}, num_of_threads (default is 2), max_size_of_field (default is 1000))
```
This will print "Complete!" after creating all pdf records in the current directory.




## License

MIT

