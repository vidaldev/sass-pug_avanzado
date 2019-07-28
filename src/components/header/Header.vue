<template lang='pug'>
    nav.columns.content-header
        <!-- Left Side -->
        .column.is-9
            #ch_box
                #ch_logo
                    img(src='https://static.platzi.com/media/user_upload/logo-d871d30b-ac23-4240-93f3-13e49084d80b.jpg')
                #ch_search
                    input(type='text' class='input_ch_search' placeholder='Busca tu peli, actor, actriz o director favorito')

        <!-- Right Slide -->
        .column.is-3
            ul.list_profile
                li.item_profile {{ perfil }}
                li.item_profile
                    img(:src="'https://ui-avatars.com/api/?name='+ perfil +'&background=50557f&color=FF535B&rounded=true&size=50'")
                li.item_profile &#9660;

</template>
//
<script>
    export default {
        name: 'content-header',
        data () {
            return {
                perfil: 'Jose Vidal'
            }
        }
    }
</script>

<style lang="scss" scoped>
    .content-header {
        height: 72px;
        background-color: #FFF;
        -webkit-box-shadow: 0px 4px 5px 0px rgba(0,0,0,0.1);
        -moz-box-shadow: 0px 4px 5px 0px rgba(0,0,0,0.1);
        box-shadow: 0px 4px 5px 0px rgba(0,0,0,0.1);
    }
    #ch_box {
        display: grid;
        align-items: center;
        grid-template-columns: 40% auto;
        height: 62px;
    }
    #ch_box  #ch_logo {
        margin: 0 0 0 35px;
    }
    #ch_box  #ch_search input {
        width: 100%;
        height: 35px;
        border-radius: 10px;
        border: 1px solid #CCC;
        padding: 0 10px;
        outline: none;
    }
    .list_profile {
        float: right;
        display: grid;
        align-items: center;
        grid-template-columns: auto auto auto;
        grid-column-gap: 5px;
        padding:5px 0;
        margin-right: 15px;
    }
    .list_profile .item_profile {
        color: #50557f;
        float: left;
        cursor:pointer;
        font-size: 16px;
        font-family: 'Lato', sans-serif;
    }
    .list_profile .item_profile:last-child{
        font-size: 12px;
    }
</style>