<template>
    <div class="baowei">
        <div class="boxTop">
            <div class="top">
            </div>
        </div>
        <div class="donghua">
            <div class="liudong">

            </div>
        </div>
        <div class="boxbot">
            <div class="bottom">
            </div>
        </div>
    </div>
</template>
  
<style>
.baowei {
    /* clear: both;
    overflow: hidden; */
    height: 150px;
    width: 150px;
}

.boxTop {
    height: 100px;
    width: 300px;
    position: relative;
    overflow: hidden;


}

.donghua {
    position: absolute;
    width: 150px;
    height: 150px;
    border-radius: 100%;
    overflow: hidden;
    top: 7px;
}

.liudong {
    animation: huadong 3s 100;
    height: 20px;
    width: 700px;
    position: absolute;
    background-image: linear-gradient(to right, red, green);
}

@keyframes huadong {
    from {
        left: 0px;
    }

    to {
        left: -300px;

    }
}

.boxbot {
    width: 300px;
    height: 50px;
    position: relative;
    overflow: hidden;

}

.top {
    width: 150px;
    height: 150px;
    background-color: aqua;
    border-radius: 100%;
    position: absolute;
}

.bottom {
    position: absolute;
    width: 150px;
    height: 150px;
    background-color: rgb(35, 56, 56);
    border-radius: 100%;
    bottom: 0px;
}
</style>
  