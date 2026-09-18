<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Para mi Princess ❤️</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    font-family: Georgia, serif;
    color: white;
    background: radial-gradient(
        circle at 50% 20%,
        #3b246b 0,
        #17102f 45%,
        #090713 100%
    );
}

.stars {
    position: fixed;
    inset: 0;
    background-image:
        radial-gradient(#fff 1px, transparent 1px),
        radial-gradient(#fff 1px, transparent 1px);
    background-size: 90px 90px, 140px 140px;
    background-position: 10px 20px, 40px 70px;
    opacity: .35;
}

.card {
    position: relative;
    width: min(92vw, 430px);
    height: 570px;
    perspective: 1400px;
    z-index: 2;
}

.letter {
    position: absolute;
    inset: 0;
    background: #fff8ef;
    color: #3d2940;
    border-radius: 18px;
    box-shadow: 0 25px 70px #0008;
    transform-style: preserve-3d;
}

.cover {
    position: absolute;
    inset: 0;
    border-radius: 18px;
    background: linear-gradient(145deg, #8e3c91, #41266f);

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    cursor: pointer;
    backface-visibility: hidden;
    z-index: 3;

    transition: transform 1.2s ease;
    transform-origin: left center;

    box-shadow: inset 0 0 0 2px #ffffff33;
}

.cover.open {
    transform: rotateY(-165deg);
}

.cover h1 {
    font-size: 34px;
    margin: 12px;
    text-align: center;
}

.cover p {
    font-size: 17px;
    opacity: .9;
}

.heart {
    font-size: 72px;
    filter: drop-shadow(0 8px 10px #0005);
}

.inside {
    position: absolute;
    inset: 0;
    padding: 30px 27px;
    overflow-y: auto;
}

.inside h2 {
    text-align: center;
    color: #7b397c;
    margin: 0 0 15px;
    font-size: 25px;
}

.inside p {
    font-size: 15.2px;
    line-height: 1.55;
    margin: 0 0 13px;
}

.signature {
    text-align: right;
    font-style: italic;
    font-weight: bold;
    color: #7b397c;
    margin-top: 18px;
}

.hint {
    position: absolute;
    bottom: 22px;
    font-family: Arial, sans-serif;
    font-size: 13px;
    opacity: .75;
}

@media (max-height: 650px) {
    .card {
        height: 88vh;
    }

    .inside {
        padding: 22px;
    }

    .inside p {
        font-size: 14px;
    }
}
</style>
</head>

<body>

<div class="stars"></div>

<div class="card">

    <div class="letter">

        <!-- CARTA POR DENTRO -->
        <div class="inside">

            <h2>Para mi princess ❤️</h2>

            <p>
                Holaaaa, feliz cumpleaños, princess de papi. ❤️
                Espero que estés bien y que estés disfrutando muchísimo
                de tu día especial.
            </p>

            <p>
                Quería felicitarte aunque sea con esta humilde carta,
                ya que no podré asistir a tu cumpleaños por motivos que
                ambos conocemos JAJAJA. Pero no quiero que te pongas triste
                ni mucho menos, quiero que disfrutes tu día como si yo
                estuviera ahí a tu lado, acompañándote y celebrando contigo.
            </p>

            <p>
                Y quién lo diría ya casi un año de relación, y además
                teniendo la oportunidad de formar parte de una fecha tan
                importante como tu cumpleaños número 18 Ya toda una adulta,
                mi bebé. 🥹❤️
            </p>

            <p>
                Solo quiero que sepas que te amo y que te amaré siempre,
                aunque quizás no sea de la forma que tú quieras o estés
                buscando. Pero al menos Dios y yo sabemos lo muchísimo
                que te amo.
            </p>

            <p>
                Espero que este nuevo año de tu vida venga lleno de
                momentos bonitos, metas cumplidas, muchas sonrisas.
            </p>

            <p>
                Aunque hoy no pueda estar físicamente contigo, quiero que
                sientas que una parte de mí está ahí celebrando contigo.
                Feliz cumpleaños, mi princess. ❤️🎂
            </p>

            <p>
                Te amo muchísimo. ❤️
            </p>

            <div class="signature">
                Att: Adrian Cruz
            </div>

        </div>

        <!-- PORTADA -->
        <div class="cover" id="cover">

            <div class="heart">💌</div>

            <h1>
                Feliz cumpleaños,<br>
                Princess de papi ❤️
            </h1>

            <p>
                Toca la carta para abrirla
            </p>

            <div class="hint">
                ✨ Una pequeña sorpresa para ti ✨
            </div>

        </div>

    </div>

</div>

<script>
const cover = document.getElementById("cover");

cover.addEventListener("click", function () {
    cover.classList.add("open");
});
</script>

</body>
</html>
