<template>
  <section>
    <h2>My Friends</h2>
    <ul>
      <li :key="friend.id" v-for="friend of friends">
        {{ friend.name }}
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  data() {
    return {
      friends: [
        {
          id: "em",
          name: "eunmin",
          phone: "101010",
          email: "test@test.com",
        },
        {
          id: "em2",
          name: "eunmin2",
          phone: "1010102",
          email: "test2@test2.com",
        },
      ],
    };
  },
};
</script>
