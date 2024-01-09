Dataset **Vineyard Rows** can be downloaded in [Supervisely format](https://developer.supervisely.com/api-references/supervisely-annotation-json-format):

 [Download](https://assets.supervisely.com/supervisely-supervisely-assets-public/teams_storage/s/m/su/5hPH3Mwty8WP5p4QI82tlWpKGEACk7LEeBtqrHcxZkwlqsNXSGzFjBcPgf6F55f0befBdlJDvfYTSA9EVPYJruhLlitsJQhGEgy24VAnzm9yrf0Gvmc53iTv2MK6.tar)

As an alternative, it can be downloaded with *dataset-tools* package:
``` bash
pip install --upgrade dataset-tools
```

... using following python code:
``` python
import dataset_tools as dtools

dtools.download(dataset='Vineyard Rows', dst_dir='~/dataset-ninja/')
```
Make sure not to overlook the [python code example](https://developer.supervisely.com/getting-started/python-sdk-tutorials/iterate-over-a-local-project) available on the Supervisely Developer Portal. It will give you a clear idea of how to effortlessly work with the downloaded dataset.

The data in original format can be [downloaded here](https://zenodo.org/api/records/4601472/files-archive).