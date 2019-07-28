<template lang='pug'>
    .column.content-movies
        .box_section(v-for="section in movies")
            .bs_title {{ section.section }}
            ul.list_movies
                li.movies_item(v-for="box in section.row" style="background-image:url('http://lorempixel.com/287/192/')") 
                    .overlay_text
                        .ot_title {{ box.name }}
                        .ot_desc {{ box.desc }}
        .github_repo
            .gr_text 
                a(href='https://github.com/vidaldev/sass-pug_avanzado/') Ir al repositorio
            .gr_img 
                a(href='https://github.com/vidaldev/sass-pug_avanzado/')
                    svg(height="50" class="octicon octicon-mark-github text-white" viewBox="0 0 16 16" version="1.1" width="50" aria-hidden="true")
                        path(fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z")
</template>

<script>
    export default {
        name: 'content-movies',
        data() {
            return {
                movies: [
                    {
                        section: 'Ahora en el cine',
                        row: [
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                        ]                        
                    }, 
                    {
                        section: 'Aclamadas por la crítica',
                        row: [
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                        ]                        
                    },
                    {
                        section: 'No te debes perder',
                        row: [
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                        ]                        
                    },
                    {
                        section: 'Favoritas del año',
                        row: [
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                            {
                                name : 'Skeleton Dance by Silly Symphonies',
                                desc : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                                img : 'skeleton.jpg' 
                            },
                        ]                        
                    }               
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .octicon {
        fill: #fff;
    }
    .box_section{
            width: 95%;
            height: auto;
            overflow: hidden;
            margin: 15px auto 30px;
    }
    .box_section .bs_title{
        font-family: 'Lato', sans-serif;
        font-weight: bold;
        font-size: 18px;
        margin-bottom: 10px;
    }
    ul.list_movies{
        width: 100%;
        padding: 0;
        margin: 0;
    }
    ul.list_movies li.movies_item {
        float: left;
        width: 287px;
        height: 192px;
        position: relative;
        margin: 0 0 30px 30px;
        cursor:pointer;
    }
    ul.list_movies li.movies_item .overlay_text{
        position: absolute;
        bottom: 0;
        width: 100%;
        height: 96px;
        background-color: rgba(255, 83, 91, 0.8);
        color: #FFF;
        font-family: 'Lato', sans-serif;
        padding: 10px;
        font-size: 14px;
    }
    ul.list_movies li.movies_item .overlay_text .ot_desc {
        font-weight: normal;
        font-size: 12px;
        margin-top: 5px;
    }
    .github_repo {
        position: fixed;
        bottom: 0;
        right: 0;
        background-color: rgba(0,0,0,0.9);
        color:#FFF;
        height: 70px;
        width: 200px;
        display: grid;
        grid-template-columns: auto 60px;
        grid-gap:15px;
        align-content: center;
    }
    .github_repo .gr_text{
        align-self: center;
        justify-self: right;
    }
    .github_repo .gr_text a{
        color: #FFF;
    }
</style>