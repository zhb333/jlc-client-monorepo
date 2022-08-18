<template>
  <div>
    <Avatar />
    <Logo />
  </div>
</template>

<script>
import { Logo, Avatar } from "@jlc/components";
import { getList, getUserInfo } from "@jlc/apis";
import { add, day } from "@jlc/utils";
export default {
  name: "IndexPage",
  components: {
    Logo,
    Avatar,
    Logo,
  },
  mounted() {
    console.log('getList', getList())
    console.log('getUserInfo', getUserInfo())
  },
  created() {
    console.log('add: ', add(1, 2))
    console.log('day: ', day())
  }
};
</script>
