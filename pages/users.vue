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
                        field: 'Primeiro Nome',
                        label: 'First Name',
                    },
                    {
                        field: 'Útimo nome',
                        label: 'Last Name',
                    },
                    {
                        field: 'Tipo de usuários',
                        label: 'user_type',
                        centered: true
                    },
                  
                ]
            }
        }
    }
</script>

<style >

#style_table{
 position: absolute;
  width: 100%;   
  padding: 18px 6% 60px 6%;
  margin: 0 0 35px 0;
  background: rgb(247, 247, 247);
  border: 1px solid rgba(147, 184, 189,0.8);
  
}

</style>
