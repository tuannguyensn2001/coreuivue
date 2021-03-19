<template>
  <div>
    <CRow>
      <CCol lg="12">
        <CTableWrapper :items="getShuffledUsersData()">
          <template #header>
            <CIcon name="cil-grid"/> Simple Table
            <div class="card-header-actions">
            </div>
          </template>
        </CTableWrapper>
      </CCol>


    </CRow>
  </div>
</template>

<script>

  import CTableWrapper from "../views/base/Table";
  import usersData from "../views/users/UsersData";
  export default {
    components: { CTableWrapper },
    methods: {
      shuffleArray (array) {
        for (let i = array.length - 1; i > 0; i--) {
          let j = Math.floor(Math.random() * (i + 1))
          let temp = array[i]
          array[i] = array[j]
          array[j] = temp
        }
        return array
      },

      getShuffledUsersData () {
        return this.shuffleArray(usersData.slice(0))
      }
    }

  }
</script>