 ### MANIFEST.MF
 
 这个文件的内容很重要，注意未行为空行
 
 
>Premain-Class: com.object.size.SizeOfObject      
 Can-Redefine-Classes: false
>````   
 
 
 ### 运行要加-javaagent
 
 ` java -javaagent:mytest.jar com.object.size.SizeOfObjectTest `
 
 ## 打包一定要用-cvfm，不能只是cvf
 
 `jar -cvfm mytest.jar MANIFEST.MF com/object/size/*` 
