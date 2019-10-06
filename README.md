# dataflow-bigtable

This repository is for blog article hosted at - [ blogger ](https://my-bigdata-blog.blogspot.com/2019/10/moving-data-from-google-storage-to-bigtable-using-dataflow.html)

In the python files you will need to update the staging and temp locations to your google storage buckets.

For input, repository has both json and avro format data for customer table (sample mysql database table). Host these to your storage buckets.

Code also has hardcoded value for bigtable instance "mybigtable".  Change in the code if you choose different name.

To run the code, clone the repo and execute command below(for bigtable).

python -m beam_gcs_bt --avro_input "your bucket location for avro input file"
--json_input "your bucket location for json input file"  --project "your project id"
