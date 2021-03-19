<template>
  <div>
    <CRow>
      <CCol xs="12" lg="12">
        <CCard>
          <CCardHeader>
            Menu chọn
            <div class="card-header-actions">
            </div>
          </CCardHeader>
          <CCardBody>
            <CTabs>
              <CTab title="Home" active>
                <Table1/>
              </CTab>
              <CTab title="Profile" >
                2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore
                et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
                aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
                dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
                officia deserunt mollit anim id est laborum.
              </CTab>
              <CTab title="Disabled" >
                3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore
                et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
                aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
                dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
                officia deserunt mollit anim id est laborum.
              </CTab>
            </CTabs>
          </CCardBody>
        </CCard>
      </CCol>

    </CRow>
  </div>
</template>

<script>
import Table1 from "../../components/Table1";
export default {
  name: 'Tabs',
  components: {Table1},
  data () {
    return {
      tabs: [
        'Calculator',
        'Shopping cart',
        'Charts'
      ],
      activeTab: 1
    }
  }
}
</script>
