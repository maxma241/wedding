<template>
  <div class="page-content">
    <!--列表元件-->
    <list></list>
  </div>
</template>
<script lang="babel!coffee" type="text/coffeescript">
  module.exports =
    mixins:  [require "components/backendbase/mixins/listConfig.coffee"]
    methods:
      listConfig: () ->
        require "components/widgetinvitation/actions/list/invitation.coffee"
      routerChange: () ->
        @init()
      init: () ->
        return
</script>
