# Parallel PDF Creation




With this tool, we can concurrently spawn multiple threads creating pdf records from a pandas dataframe.


## Installation


```sh
pip install parallel_pdf_creation

```


After installation, use it directly in the jupyter notebook as,
```
import parallel_pdf_creation as ppc

ppc.begin({"name_of_df1": df1, "name_of_df2": df2, .....}, num_of_threads (default is 2), max_size_of_field (default is 1000))
```
This will print "Complete!" after creating all pdf records in the current directory.




## License

MIT

