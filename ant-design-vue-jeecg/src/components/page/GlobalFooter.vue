<template>
  <div class="footer">
    <div class="copyright">
      Copyright
      <a-icon type="copyright"/>
      2014-{{year}} <span>捷特软件 出品</span>
    </div>
  </div>
</template>

<script>
  export default {
    name: "LayoutFooter",
    data() {
      return {
        
      }
    },
    computed: {
      year() {
        return new Date().getFullYear();
      }
    },
  }
</script>

<style lang="less" scoped>
  .footer {
    padding: 0 16px;
    margin: 48px 0 24px;
    text-align: center;

    .links {
      margin-bottom: 8px;

      a {
        color: rgba(0, 0, 0, .45);

        &:hover {
          color: rgba(0, 0, 0, .65);
        }

        &:not(:last-child) {
          margin-right: 40px;
        }
      }
    }
    .copyright {
      color: rgba(0, 0, 0, .45);
      font-size: 14px;
    }
  }
</style>