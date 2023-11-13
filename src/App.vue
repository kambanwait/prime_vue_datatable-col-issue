<script setup>
import DataTable from 'primevue/datatable';
import Column from 'primevue/column';
import { ref } from "vue";

const allUsers = ref([
    {
        "id": "6c41d80b-7743-11ee-b647-62239528fd2e",
        "name": "gmorrison",
        "email": "gmorrison@coade3.com",
        "password": "",
        "sysadmin": true,
        "roles": [
            {
                "id": "33699aee-7743-11ee-b647-62239528fd2e",
                "name": "test manager"
            }
        ],
        "functions": []
    },
    {
        "id": "a3b8abea-78c9-11ee-b647-62239528fd2e",
        "name": "NotAdmin22",
        "email": "notadmin@email.com",
        "password": "",
        "sysadmin": false,
        "roles": [
            {
                "id": "3a4efd77-7743-11ee-b647-62239528fd2e",
                "name": "lead tester"
            }
        ],
        "functions": []
    },
    {
        "id": "7e797b09-7a42-11ee-b647-62239528fd2e",
        "name": "notadmin3bb",
        "email": "notadmin3@email.com",
        "password": "",
        "sysadmin": false,
        "roles": [
            {
                "id": "",
                "name": "n/a"
            }
        ],
        "functions": []
    },
    {
        "id": "97adb398-7d5a-11ee-b647-62239528fd2e",
        "name": "Kam Admin",
        "email": "notadmin@email.com",
        "password": "",
        "sysadmin": true,
        "roles": [
            {
                "id": "33699aee-7743-11ee-b647-62239528fd2e",
                "name": "test manager"
            }
        ],
        "functions": []
    },
    {
        "id": "b384d455-7f0e-11ee-b647-62239528fd2e",
        "name": "gmtester",
        "email": "gmtester@xte.co.uk",
        "password": "",
        "sysadmin": false,
        "roles": [
            {
                "id": "3cb2687f-7743-11ee-b647-62239528fd2e",
                "name": "tester"
            }
        ],
        "functions": []
    },
    {
        "id": "8f6149ba-7f12-11ee-b647-62239528fd2e",
        "name": "asdasdad",
        "email": "asdasd@asdasd.com",
        "password": "",
        "sysadmin": false,
        "roles": [
            {
                "id": "3a4efd77-7743-11ee-b647-62239528fd2e",
                "name": "lead tester"
            }
        ],
        "functions": []
    }
]);
</script>

<template>
  <div class="card">
    <DataTable
      :value="allUsers"
    >
      <Column field="roles" header="Role" style="width: 25%" />
      <Column field="roles[0].id" header="Role" style="width: 25%" />
    </DataTable>
  </div>
</template>