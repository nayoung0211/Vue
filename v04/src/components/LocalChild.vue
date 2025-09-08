<template>
    <div>
        나는 Child Components 입니다 
        <input type ="text" ref="myInput">
        <button @click="$emit('createPost')">부모 이벤트 호출</button>
    </div>
    </template>