# k8s_config

This is a simple module that supports creating or removing vDCs. A vDC is required before you can create servers. This module has a dependency on ionos-cloud &gt;= 6.0.0

## Example Syntax


```yaml

  - name: Get k8s config
  k8s_config:
    k8s_cluster_id: "ed67d8b3-63c2-4abe-9bf0-073cee7739c9"
    config_file: 'config.yaml'
  
```
&nbsp;

&nbsp;

# state: **present**
```yaml
  
  - name: Get k8s config
  k8s_config:
    k8s_cluster_id: "ed67d8b3-63c2-4abe-9bf0-073cee7739c9"
    config_file: 'config.yaml'
  
```
### Available parameters for state **present**:
&nbsp;

  | Name | Required | Type | Default | Description |
  | :--- | :---: | :--- | :--- | :--- |
  | k8s_cluster_id | True | str |  | The ID of the K8s cluster. |
  | config_file | True | str |  | The name of the file in which to save the config. |
  | api_url | False | str |  | The Ionos API base URL. |
  | username | True | str |  | The Ionos username. Overrides the IONOS_USERNAME environment variable. |
  | password | True | str |  | The Ionos password. Overrides the IONOS_PASSWORD environment variable. |
  | wait | False | bool | True | Wait for the resource to be created before returning. |
  | wait_timeout | False | int | 600 | How long before wait gives up, in seconds. |
  | state | False | str | present | Indicate desired state of the resource. |

&nbsp;

&nbsp;