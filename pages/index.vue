<template>
  <section class="container">
    <b-navbar toggleable="lg" type="light" variant="success">
      <b-navbar-brand href="#" thread-class="text-white">
        Todo List
      </b-navbar-brand>
      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template v-slot:button-content>
              <em>User</em>
            </template>
            <b-dropdown-item href="#">
              Sign Out
            </b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <table class="Lists">
      <thead>
        <tr>
          <th>タスク</th>
          <th>登録日時</th>
          <th>状態</th>
          <th></th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>テスト</td>
          <td>2020-06-1 17:00</td>
          <td>
            <button class="button button--edit">
              編集
            </button>
          </td>
          <td>
            <button class="button button--delete">
              削除
            </button>
          </td>
        </tr>
      </tbody>
    </table>
    <div class="addArea">
      <input
        id="addName"
        type="text"
        name="addName"
        placeholder="タスクを入力してください"
      />
      <button id="addButton" class="button button--green">
        追加
      </button>
    </div>
  </section>
</template>

<script>
import Login from '~/components/login/login.vue'

// export default {
//   components: {
//     Login,
//   },
// }
</script>

<style></style>
