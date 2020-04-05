#### HBaseStorage.java

```java
	public void createTable(String tablename,String families) throws IOException {/////
		TableName tableName2 = TableName.valueOf(tablename);
		if(!admin.tableExists(tableName2)) {
			logger.info("开始建表");
			HTableDescriptor hTableDescriptor = new HTableDescriptor(tableName2);
			for(String f : families.split(",")) {
				HColumnDescriptor hColumnDescriptor = new HColumnDescriptor(f);
				hTableDescriptor.addFamily(hColumnDescriptor);
			}
			admin.createTable(hTableDescriptor);
			logger.info("创建成功");
		} else {
			logger.info("表以存在");
		}
	}
```

