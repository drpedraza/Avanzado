<script>
    export let title;
    export let color;
    export let text;

</script>
<main>
    <div class="Note">
        <div class="Note-container" style={'background-color: ' + color}>
            <div class="header">
                <div class="options">
                    <button><svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><g><rect fill="none" height="24" width="24"/></g><g><path d="M12,2C6.49,2,2,6.49,2,12s4.49,10,10,10c1.38,0,2.5-1.12,2.5-2.5c0-0.61-0.23-1.2-0.64-1.67c-0.08-0.1-0.13-0.21-0.13-0.33 c0-0.28,0.22-0.5,0.5-0.5H16c3.31,0,6-2.69,6-6C22,6.04,17.51,2,12,2z M17.5,13c-0.83,0-1.5-0.67-1.5-1.5c0-0.83,0.67-1.5,1.5-1.5 s1.5,0.67,1.5,1.5C19,12.33,18.33,13,17.5,13z M14.5,9C13.67,9,13,8.33,13,7.5C13,6.67,13.67,6,14.5,6S16,6.67,16,7.5 C16,8.33,15.33,9,14.5,9z M5,11.5C5,10.67,5.67,10,6.5,10S8,10.67,8,11.5C8,12.33,7.33,13,6.5,13S5,12.33,5,11.5z M11,7.5 C11,8.33,10.33,9,9.5,9S8,8.33,8,7.5C8,6.67,8.67,6,9.5,6S11,6.67,11,7.5z"/></g></svg></button>
                    <button><svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M16 9v10H8V9h8m-1.5-6h-5l-1 1H5v2h14V4h-3.5l-1-1zM18 7H6v12c0 1.1.9 2 2 2h8c1.1 0 2-.9 2-2V7z"/></svg></button>
                </div>
                <br>
            </div>
            <div class="content">
                <div class="title">
                    <input type="text" placeholder="Sin titulo..." bind:value={title}>
                </div>
                <br>
                <div class="text">
                    <textarea bind:value={text} cols="30" rows="10" placeholder="Escribir..."></textarea>
                </div>
            </div>
        </div>
    </div>
</main>
<style>
    .Note{
        background-color: white;
        border-radius: 3px;
        border: solid 2px transparent;
        overflow: hidden;
        height: 400px;
    }
    .Note-container{
        height: 100%;
    }
    .Note:focus-within{
        border: solid 2px #000;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
    }
    .Note .Note-container .header{
        padding: 5px;
    }
    .Note .options{
        display: flex;
        justify-content: space-between;
    }
    .Note .content{
        padding: 0 20px;
    }
    .text textarea{
        width: 100%;
        border: 0;
        outline: none;
        resize: none;
        height: 250px;
    }

    .title input{
        font-size: 22px;
        font-weight: bold;
        padding: 10px 0;
        outline: none;
        border: none;
        width: 100%;
    }
    button{
        margin: 0;
        border: none;
        background-color: transparent;
        cursor: pointer;
    }
    textarea, input{
        background: transparent;
    }
    </style>