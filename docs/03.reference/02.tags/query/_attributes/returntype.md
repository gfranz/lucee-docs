one of the following values:
			- query: default for all dbtype expect "hql", returns a query object
			- array_of_entity: works only with dbtype "hql" and is also the default value for dbtype "hql"
			- struct: returns a struct with the keys containing the values of the field set with the attribute columnKey and the values being a struct of the record
			- array: returns an array of record structs
