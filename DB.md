DB:

 1. 每个表应使用制表符分隔文本存储在单独的文件中。
 2. 每行的值id不会由用户提供，而是由服务器自动生成。
 3. 表名应该不区分大小写（因为某些文件系统在区分大小写方面存在问题）。用户提供的任何表名在保存到文件系统之前都应转换为小写。
 4. 您应该将列名称视为不区分大小写以进行查询，但您应该在存储它们时保留大小写（以便用户可以根据需要使用 CamelCase）。
 5. 您应该使用File.separator常量