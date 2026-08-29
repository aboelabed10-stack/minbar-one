<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>تسجيل الدخول | منبر ون</title>

<style>

*{
    box-sizing:border-box;
    margin:0;
    padding:0;
    font-family:Tahoma,Arial,sans-serif;
}

body{
    min-height:100vh;

    display:flex;
    align-items:center;
    justify-content:center;

    padding:20px;

    background:
    radial-gradient(circle at 10% 20%,#dfe8ff,transparent 30%),
    radial-gradient(circle at 90% 80%,#eee3ff,transparent 30%),
    #f7f9ff;
}

.card{
    width:100%;
    max-width:430px;

    background:white;

    padding:35px;

    border-radius:25px;

    box-shadow:0 20px 60px rgba(40,60,120,.13);
}

.logo{
    width:65px;
    height:65px;

    margin:0 auto 15px;

    border-radius:20px;

    display:grid;
    place-items:center;

    color:white;

    font-size:32px;
    font-weight:bold;

    background:linear-gradient(135deg,#4f7cff,#7c5cff);
}

h1{
    text-align:center;

    color:#17213a;

    margin-bottom:7px;
}

.subtitle{
    text-align:center;

    color:#718096;

    font-size:13px;

    margin-bottom:28px;
}

label{
    display:block;

    margin-bottom:7px;

    color:#344054;

    font-size:13px;

    font-weight:bold;
}

input{
    width:100%;

    padding:14px;

    margin-bottom:17px;

    border:1px solid #e2e7f0;

    border-radius:12px;

    outline:none;

    font-size:14px;

    direction:rtl;
}

input:focus{
    border-color:#4f7cff;

    box-shadow:0 0 0 3px rgba(79,124,255,.1);
}

button{
    width:100%;

    padding:14px;

    border:0;

    border-radius:12px;

    background:linear-gradient(135deg,#4f7cff,#7c5cff);

    color:white;

    font-size:15px;

    font-weight:bold;

    cursor:pointer;

    transition:.2s;
}

button:hover{
    transform:translateY(-2px);
}

.back{
    display:block;

    text-align:center;

    margin-top:20px;

    color:#4f7cff;

    text-decoration:none;

    font-size:13px;
}

.math{
    text-align:center;

    margin-top:25px;

    color:#9aa5ba;

    font-size:22px;

    word-spacing:12px;
}

</style>
</head>

<body>

<div class="card">

<div class="logo">
∑
</div>

<h1>
أهلًا بك في منبر ون 👋
</h1>

<p class="subtitle">
سجّل دخولك وابدأ رحلة التفوق في الرياضيات 🎓
</p>


<form id="loginForm">

<label>
البريد الإلكتروني
</label>

<input
type="email"
id="email"
placeholder="example@email.com"
required
>


<label>
كلمة المرور
</label>

<input
type="password"
id="password"
placeholder="أدخل كلمة المرور"
required
>


<button type="submit">
🚀 تسجيل الدخول
</button>

</form>


<a class="back" href="index.html">
← العودة إلى الصفحة الرئيسية
</a>


<div class="math">
π √ ∑ x² ∞ ÷
</div>

</div>


<script>

document.getElementById("loginForm").addEventListener("submit",function(e){

e.preventDefault();

alert(
"🔐 سيتم تفعيل تسجيل الدخول الحقيقي وربطه بحساب الطالب في الخطوة التالية."
);

});

</script>

</body>
</html>
