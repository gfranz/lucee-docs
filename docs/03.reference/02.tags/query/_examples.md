```luceetag+trycf
<cfquery name="qry" datasource="myDatasource">
  SELECT id, name, firstName, telephone FROM addresses WHERE name = 'Balboa' and firstName='Rocky'
</cfquery>
<cfdump eval=qry>

<!--- returning a struct as a struct containing one record struct for each key set by columnKey --->
<cfquery name="str" datasource="myDatasource" returnType="struct" columnKey="id">
  SELECT id, name, firstName, telephone FROM addresses WHERE name = 'Balboa' and firstName='Rocky'
</cfquery>
<cfdump eval=str>

<!--- returning an array containing one record struct for each rownumber --->
<cfquery name="arr" datasource="myDatasource" returnType="struct" columnKey="id">
  SELECT id, name, firstName, telephone FROM addresses WHERE name = 'Balboa' and firstName='Rocky'
</cfquery>
<cfdump eval=arr>

```
