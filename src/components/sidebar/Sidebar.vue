<template lang='pug'>
    .column.content-sidebar
        ul.menu_sidebar_top
            li.mst_item(v-for="mtop in menu_top")
                .msti_img
                    i.material-icons {{ mtop.icon }}
                .msti_text {{ mtop.text }}
        ul.menu_sidebar_bottom
            li.mst_item(v-for="mbottom in menu_bottom")
                .msti_img
                    i.material-icons {{ mbottom.icon }}
                .msti_text {{ mbottom.text }} 
</template>

<script>
    export default {
        name: 'content-sidebar',
        data() {
            return {
                menu_top: [
                    {
                        icon: 'home',
                        text: 'Home'
                    },
                    {
                        icon: 'whatshot',
                        text: 'Trending'
                    },
                    {
                        icon: 'favorite',
                        text: 'Más likes'
                    }
                ],
                menu_bottom: [
                    {
                        icon: 'settings',
                        text: 'Ajustes'
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    @import url('https://fonts.googleapis.com/icon?family=Material+Icons');

    .content-sidebar{
        position:fixed;
        width: 89px;
        height: calc(100% - 60px);
        background: rgba(255,83,92,1);
        background: -moz-linear-gradient(left, rgba(255,83,92,1) 0%, rgba(253,115,108,1) 100%);
        background: -webkit-gradient(left top, right top, color-stop(0%, rgba(255,83,92,1)), color-stop(100%, rgba(253,115,108,1)));
        background: -webkit-linear-gradient(left, rgba(255,83,92,1) 0%, rgba(253,115,108,1) 100%);
        background: -o-linear-gradient(left, rgba(255,83,92,1) 0%, rgba(253,115,108,1) 100%);
        background: -ms-linear-gradient(left, rgba(255,83,92,1) 0%, rgba(253,115,108,1) 100%);
        background: linear-gradient(to right, rgba(255,83,92,1) 0%, rgba(253,115,108,1) 100%);
        display: grid;
        grid-template-rows: auto auto;
    }
    .mst_item {
        color: #FFF;
        text-align: center;
        font-family: 'Lato', sans-serif;
        font-size: 12px;
        margin-bottom: 20px;
        cursor: pointer;
    }
    .mst_item .msti_text{
        margin-top: -8px;
    }
    .material-icons{
        font-size: 47px;
    }
    .menu_sidebar_bottom {
        align-self: end;
    }
    .menu_sidebar_bottom .mst_item {
        margin-bottom: 0;
    }
</style>