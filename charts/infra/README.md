# Infrastructure Chart

This Helm Chart includes a set of templates to setting up an Openshift cluster generating the following elements:

* Namespaces
* Resource Quotas
* Network Policies

## Testing

The file _values-test.yaml_ is very important to test all the functionality implement in the chart. By default, the file _value.yaml_ is empty in order to not generate files that could not be necessary in all the Openshift Clusters for every environment.

Please execute the following command in the CI process to test the chart functionality:

```$bash
helm template . -f values-test.yaml
```

## Author

Asier Cidon @RedHat