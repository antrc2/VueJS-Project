<template>
    <div class="container mt-5">
        <h1 class="text-center">Danh sách sản phẩm</h1>
        <div class="row">
            <div class="col-sm-4">
                <div class="card">
                    <img :src="products[0].image" alt="Hình ảnh sản phẩm" class="card-img-top">
                    <div class="card-body">
                        <h3 class="card-title">{{ products[0].name }}</h3>
                        <p class="card-text">{{ products[0].description }}</p>
                        <p class="card-text">Giá: {{ products[0].price }}</p>
                        <button class="btn btn-success">Mua ngay</button>
                    </div>
                </div>
            </div>
            <div class="col-sm-4">
                <div class="card">
                    <img :src="products[1].image" alt="Hình ảnh sản phẩm" class="card-img-top">
                    <div class="card-body">
                        <h3 class="card-title">{{ products[1].name }}</h3>
                        <p class="card-text">{{ products[1].description }}</p>
                        <p class="card-text">Giá: {{ products[1].price }}</p>
                        <button class="btn btn-success">Mua ngay</button>
                    </div>
                </div>
            </div>
            <div class="col-sm-4">
                <div class="card">
                    <img :src="products[2].image" alt="Hình ảnh sản phẩm" class="card-img-top">
                    <div class="card-body">
                        <h3 class="card-title">{{ products[2].name }}</h3>
                        <p class="card-text">{{ products[2].description }}</p>
                        <p class="card-text">Giá: {{ products[2].price }}</p>
                        <button class="btn btn-success">Mua ngay</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
const products = [
    {
        name: "Sản phẩm 1",
        description: "Mô tả sản phẩm 1, rất chất lượng và đáng mua",
        price: 500000,
        image: "https://picsum.photos/id/1/300/300.jpg"
    },
    {
        name: "Sản phẩm 2",
        description: "Mô tả sản phẩm 2, chất lượng tốt và giá phải chăng",
        price: 300000,
        image: "https://picsum.photos/id/2/300/300.jpg"
    },
    {
        name: "Sản phẩm 3",
        description: "Mô tả sản phẩm 3, sản phẩm cao cấp và nhiều tính năng",
        price: 1000000,
        image: "https://picsum.photos/id/3/300/300.jpg"
    }
    
]
</script>

<style lang="scss" scoped>

</style>