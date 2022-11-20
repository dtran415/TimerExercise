function countDown(num) {
    const id = setInterval(function() {
        num--;
        if (num > 0) {
            console.log(num)
        } else {
            clearInterval(id);
            console.log("DONE!");
        }
    }, 1000)
}

function randomGame() {
    let count = 0;
    const id = setInterval(function() {
        let num = Math.random();
        count++;
        if (num > 0.75) {
            clearInterval(id);
            console.log(count);
        }
    }, 1000)
}