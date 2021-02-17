# Testlib for Lemons

Testlib for Lemons 添加了 Testlib 对本地自定义测试和 Lemon 系评测软件的 Special Judge 的支持。

对于本地自定义测试，可以使用 `registerLocalChecker(<Input_File>, <Output_File>, <Answer_File>, <Perfect_Score>, <Score_File>[, <Report_File>])` 的格式进行初始化，其中 `<Perfect_Score>` 表示该测试点的满分，`<Score_File>` 表示将该测试点得分输出到的文件的文件名，`<Report_File>` 表示附加信息的输出位置，可以不填（如果不填则不会输出附加信息）。

对于 Lemon 系评测软件的 Special Judge，可以直接使用 `registerLemonChecker(argc, argv)`，类似正常使用 Testlib 的 checker 功能时的操作。
