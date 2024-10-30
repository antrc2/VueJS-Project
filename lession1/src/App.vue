<script setup>
const user = {
  "maSinhVien": "PH53674",
  "name": "Nguyễn Ngọc An",
  "address": "Hà Nội"
}
</script>

<template>
<div>
  <table class="table">
    <thead>
      <tr>
        <th>Mã Sinh viên</th>
        <th>Họ và tên</th>
        <th>Địa chỉ</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>{{ user.maSinhVien }}</td>
        <td>{{ user.name }}</td>
        <td>{{ user.address }}</td>
      </tr>
    </tbody>
  </table>
</div>
</template>

<style scoped>

</style>
