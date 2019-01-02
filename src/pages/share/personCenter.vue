<template>
    <div>

        <group>
            <cell @cell-label-color="red" title="我的订单" is-link value="查看全部订单"></cell>
            <grid :show-vertical-dividers="false" :show-lr-borders="false">
                <grid-item label="订单" v-for="i in 4">
                    <img slot="icon" src="../../assets/logo.png">
                </grid-item>
            </grid>
        </group>
        <group>
            <cell title="地址管理" is-link></cell>
        </group>
    </div>
</template>

<script>
    import { XHeader, Group, Cell,XButton, Grid, GridItem  } from 'vux'
    export default {
        name: "person-center",
        components: {
            XHeader,
            Group,
            Cell,
            XButton,
            Grid,
            GridItem
        }
    }
</script>

<style>
    .weui-grid{
        text-decoration: none;
    }
    .weui-grid:before{
        border:none;
    }
</style>
<style scoped>

</style>
