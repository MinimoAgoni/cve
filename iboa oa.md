SQL injection vulnerability exists in  IBOS OA v4.5.5 

official website:http://www.ibos.com.cn/

route:?r=recruit/interview/export&interviews=x

1.Function point: Integrated office = "Recruitment management =" Interview management = "Export

![(1)](https://github.com/MinimoAgoni/cve/assets/129938010/354a436e-fad4-4913-98f1-6a8a0f26cbf7)

![(2)](https://github.com/MinimoAgoni/cve/assets/129938010/a719a5ff-68ee-4142-bf3f-858b33f7d6a6)

2.The actionExport() method is found, and the interviews parameters obtained are directly brought to fetchAll() under the model layer for data processing.

![(3)](https://github.com/MinimoAgoni/cve/assets/129938010/d4ecdb32-1902-4b8d-a551-fcc8907b5917)

There are still some encapsulation processing operations of the method

![(4)](https://github.com/MinimoAgoni/cve/assets/129938010/514d98a6-1d29-4421-b716-7ac44a3a8413)

![(5)](https://github.com/MinimoAgoni/cve/assets/129938010/039c21a4-6569-4c7b-b931-2e280f4ab631)
