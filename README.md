<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title> Hover sản phẩm </title>
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
<body>
    <div class="card">
        <div class="card_heart">
            <i class='bx bx-heart-circle'></i>
        <div>
        <div class="card_cart">
            <i class='bx bx-cart-add' ></i>
        </div>
        <div class="card_img">
            <img src="https://static.wixstatic.com/media/94e66f_56e0d5db89a74dbcb3ba2896c67bbc8e~mv2_d_1500_1500_s_2.png/v1/fill/w_380,h_380,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/94e66f_56e0d5db89a74dbcb3ba2896c67bbc8e~mv2_d_1500_1500_s_2.png" alt="" srcset="">
        <div></div>
        <div class="card_title">
            Giỏ Snack
        </div>
        <div class="card_price">50.000 VNĐ</div>
        <div class="card_size">
            <h3>Số lượng</h3>
            <span>1</span>
            <span>2</span>
            <span>3</span>
        </div>
        <div class="card_color">
            <h3>Màu sắc</h3>
            <span class="card_color_green"></span>
            <span class="card_color_red"></span>
            <span class="card_color_yellow"></span>
        </div>
        <div class="card_action">
            <button>Mua</button>
            <button>Thêm vào giỏ</button>
        </div>
    </div>
    

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
:root{
    --primary-color: rgb(131, 213, 131 );
}

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    height: 100vh;
    font-family: "Poppins", sans-serif;
    background: linear-gradient(115deg, rgb(24, 21, 78) 0%, rgb(57, 55, 190) 0%, rgba(173,145,84,1) 100%, rgba(82,117,88,0.9189189189189189) 100%);
}

.card {
    margin: 150px auto;
    width: 300px;
    height: 500px;
    background: #F8E0F7;
    padding: 20px;
    border-radius: 15px;
    position: relative;
}
.card_heart,.card_cart {
    font-size: 25px;
    position: absolute;/*xác định vị trí trong css*/
    left: 20px;
    top: 15px;
    cursor: pointer;/*hiển thị bàn tay khi di chuột vào*/
}

.card_heart {
    color: red;
    right: unset;
    left: 20px;
}

.card_cart {
    left: unset;
    right: 20px;
    color: black;
    top: 0px;
}

.card_img {
    width: 90%;
    transition: 0.5s;
}
.card_img img {
    width: 100%;
    height: 100%;
    object-fit: cover;/*ảnh to nhưng sẽ tự co vào*/
}

.cart_title, .card_price {
    font-size: 25px;
    font-weight: bold;
    text-align: center;
    transition: 0.5s;

}

.card_title {
    color: #0000FF;
    text-align: center;
    font-weight: bold;
}
.card_size, .card_color {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
    color: black;
    font-size: medium;
}

.card_size span {
    padding: 1px 10px;
    background: #A9BCF5;
    color: black;
    border-radius: 5px;
    margin: 0 5px;
    cursor: pointer;
}

.card_color span {
    width: 15px;
    height: 15px;
    border-radius: 50%;
    margin: 0 5px;
    cursor: pointer;
}

.card_color_green {
    background: green;
}
.card_color_red {
    background: red;
}
.card_color_yellow {
    background: rgb(202, 232, 9);
}

.card_action button {
    background: var(--primary-color);
    border: none;
    outline: none;
    color: aliceblue;
    padding: 10px 20px;
    border-radius: 5px;
    font-weight: bold;
    margin-right: 10px;
    transition: 0.25s;
    cursor: pointer;
}
.card_action button:hover {
    transform: scale(0.9);
}

.card:hover .card_img {
    transform: translateY(-90px) rotate(-20deg);
}

.card:hover .card_title {
    transform: translate(-35px, -70px);
}

.card:hover .card_price {
    transform: translate(-117px, -72px);
}

.card_size {
    margin-top: 150px;
    visibility: hidden;
    opacity: 0;
}

.card_size, .card_color, .card_action {
    visibility: hidden;
    opacity: 0;
    transition: 0.5s;
    transition-delay: 0.4s;
}

.card:hover .card_size,
.card:hover .card_color,
.card:hover .card_action {
    visibility: visible;
    opacity: 100;
}

.card:hover .card_size {
    margin-top: -30px;
}
    </style>
<script>
    src="https://cdn.jsdelivr.net/npm/boxicons@2.1.4/boxicón.min.js"
</script>

</body>
</html>
