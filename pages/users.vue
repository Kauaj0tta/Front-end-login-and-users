<template>
<div id="style_table">
      <b-table :data="data" :columns="columns"></b-table>
</div>
  
</template>

<script>
    export default {
        data() {
            return {
                data: [
                    { 'id': 1, 'first_name': 'Jesse', 'last_name': 'Simmons', 'user_type': 'adm', },
                    { 'id': 2, 'first_name': 'John', 'last_name': 'Jacobs', 'user_type': 'professor', },
                    { 'id': 3, 'first_name': 'Tina', 'last_name': 'Gilbert', 'user_type': 'infermeiro', },
                    { 'id': 4, 'first_name': 'Clarence', 'last_name': 'Flores','user_type': 'aluno', },
                    { 'id': 5, 'first_name': 'Anne', 'last_name': 'Lee',  'user_type': 'aluno' }
                ],
                columns: [
                    {
                        field: 'id',
                        label: 'ID',
                        width: '40',
                        numeric: true
                    },
                    {
                        field: 'first_name',
                        label: 'First Name',
                    },
                    {
                        field: 'last_name',
                        label: 'Last Name',
                    },
                    {
                        field: 'user_type',
                        label: 'Type of user',
                        centered: true
                    },
                  
                ]
            }
        }
    }
</script>

<style >
*, *:before, *:after { 
  margin:0;
  padding:0;
  font-family: Arial,sans-serif;
}

body{
  margin:10px;
}


#style_table{
position: absolute;
  width: 90%;   
  padding: 20px 7% 60px 7%;
  margin: 0 0 35px 0;
  background: rgb(255, 253, 253);
  border-radius: 15px;

 
  
}

</style>
