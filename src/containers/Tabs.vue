<template>
    <div class="tabs-warp" flex="dir:top">
        <router-view flex-box="1"></router-view>
        <div class="tabs" flex-box="0" flex="dir:left">
            <router-link class="tab" :to="{path:'/tabs/index'}"
                         active-class="tab-active"
                         replace flex-box="1">首页</router-link>
            <router-link class="tab" :to="{path:'/tabs/financial'}"
                         active-class="tab-active"
                         replace flex-box="1">理财</router-link>
            <router-link class="tab" :to="{path:'/tabs/my'}"
                         active-class="tab-active"
                         replace flex-box="1">我的</router-link>
        </div>
    </div>
</template>

<script>
    import '../less/tabs.less';
    export default {
        name: 'tabs'
    }
</script>
