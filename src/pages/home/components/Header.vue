<template>
    <div>
        <div class="header">
            <div class="header-left">
                <div class="iconfont back-icon">&#xec45;</div>
                </div>
            <div class="header-input">
                <span class="iconfont big-icon">&#xec13;</span>
                输入城市/景点/游
                玩主题
            </div>
            <router-link to='/city'>
                <div class="header-right">
                    {{this.city}}
                    <span class="iconfont">&#xec0b;</span>
                </div>
            </router-link>    
        </div>
       
    </div>
</template>


<script>
export default {
        name:'HomeHeader',
        props:{
            city:String
        }
}
</script>


<style lang="stylus" scoped>
// 1rem = html font-size = 50px

@import "~styles/varibles.styl";
.header
    line-height:$headerHeight
    display:flex
    background:$bgColor
    color:#fff 
    .header-left
        width:.64rem
        float:left
        .back-icon
            text-align:center
            font-size:0.4rem 
    .header-input
        flex:1
        background:#fff
        border-radius 0.1rem
        margin-top:.12rem
        height:0.64rem
        line-height:.64rem 
        margin-left:.2rem
        color:#ccc
        padding-left:.2rem

        .big-icon
            font-size:0.4rem 

    .header-right
        width:1.24rem
        float:right
        text-align:center 
        color :#fff   

</style>

