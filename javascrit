// ==========================================
// STUDYIA - ASISTENTE INTELIGENTE
// ==========================================


// ELEMENTOS DEL HTML

const subject = document.getElementById("subject");

const question = document.getElementById("question");

const askButton = document.getElementById("askButton");

const answerSection = document.getElementById("answerSection");

const answerText = document.getElementById("answerText");

const answerSubject = document.getElementById("answerSubject");

const errorMessage = document.getElementById("errorMessage");

const history = document.getElementById("history");

const emptyHistory = document.getElementById("emptyHistory");

const clearHistory = document.getElementById("clearHistory");

const themeButton = document.getElementById("themeButton");

const counter = document.getElementById("counter");

const summaryButton = document.getElementById("summaryButton");


// ==========================================
// CONTADOR DE CARACTERES
// ==========================================

question.addEventListener("input", function () {

    counter.textContent = question.value.length;

});


// ==========================================
// FUNCION PARA GENERAR RESPUESTAS
// ==========================================

function generateAnswer(subject, question) {

    const q = question.toLowerCase();


    // MATEMÁTICA

    if (subject === "Matemática") {

        if (
            q.includes("ecuación") ||
            q.includes("ecuaciones")
        ) {

            return `Una ecuación es una igualdad matemática que contiene una o más incógnitas.

Para resolverla, primero hay que dejar la incógnita sola en un lado de la igualdad.

Por ejemplo:

2x + 4 = 10

Primero restamos 4:

2x = 6

Después dividimos por 2:

x = 3

Por lo tanto, la solución es x = 3.`;

        }

        if (
            q.includes("porcentaje") ||
            q.includes("%")
        ) {

            return `Para calcular un porcentaje podés multiplicar el número por el porcentaje y dividirlo por 100.

Por ejemplo:

20% de 150

150 × 20 ÷ 100 = 30

Entonces, el 20% de 150 es 30.`;

        }

        return `En Matemática, lo mejor es identificar primero qué te está pidiendo el ejercicio.

Después podés separar los datos, elegir la fórmula o procedimiento necesario y resolverlo paso a paso.

Si me das un ejercicio específico, puedo ayudarte a resolverlo.`;

    }


    // HISTORIA

    if (subject === "Historia") {

        if (
            q.includes("malvinas") ||
            q.includes("guerra")
        ) {

            return `La Guerra de Malvinas ocurrió en 1982 entre Argentina y el Reino Unido.

El conflicto comenzó el 2 de abril de 1982, cuando las fuerzas argentinas desembarcaron en las islas.

La guerra terminó el 14 de junio de 1982 con la rendición argentina.

El conflicto tuvo importantes consecuencias políticas y sociales tanto en Argentina como en el Reino Unido.`;

        }

        if (
            q.includes("revolución francesa")
        ) {

            return `La Revolución Francesa comenzó en 1789.

Fue un proceso político y social que terminó con el antiguo régimen en Francia.

Entre sus causas estuvieron las desigualdades sociales, los problemas económicos y las ideas de la Ilustración.

Uno de sus acontecimientos más conocidos fue la toma de la Bastilla.`;

        }

        return `La Historia estudia hechos y procesos ocurridos en el pasado.

Para comprender un acontecimiento histórico es importante tener en cuenta sus causas, su desarrollo y sus consecuencias.

También es útil ubicarlo en un lugar y período determinado.`;

    }


    // INGLÉS

    if (subject === "Inglés") {

        if (
            q.includes("present simple") ||
            q.includes("presente simple")
        ) {

            return `El Present Simple se utiliza principalmente para hablar de hábitos, rutinas y hechos generales.

Ejemplo:

I play football every Saturday.

En tercera persona singular (he, she, it), generalmente se agrega -s al verbo:

She plays football.

Para preguntas podemos utilizar DO o DOES.

Do you play football?

Does she play football?`;

        }

        if (
            q.includes("past simple") ||
            q.includes("pasado simple")
        ) {

            return `El Past Simple se utiliza para hablar de acciones que ocurrieron y terminaron en el pasado.

Ejemplo:

I visited London last year.

En los verbos regulares generalmente se agrega -ed.

Visit → Visited

Algunos verbos son irregulares:

Go → Went

Eat → Ate

See → Saw`;

        }

        return `En Inglés es importante observar el tiempo verbal de la oración.

Algunas palabras que pueden ayudarte son:

Present Simple → every day, usually, always.

Past Simple → yesterday, last week, ago.

Present Continuous → now, at the moment.

Si me escribís una oración, puedo explicarte cómo funciona.`;

    }


    // TECNOLOGÍA

    if (subject === "Tecnología") {

        if (
            q.includes("ia") ||
            q.includes("inteligencia artificial")
        ) {

            return `La Inteligencia Artificial (IA) es una tecnología que permite desarrollar sistemas capaces de realizar tareas que normalmente requieren capacidades humanas.

Por ejemplo, una IA puede analizar información, reconocer imágenes, comprender textos o generar respuestas.

En este proyecto, la IA se utiliza como asistente para responder preguntas de los estudiantes.`;

        }

        if (
            q.includes("red") ||
            q.includes("internet")
        ) {

            return `Una red informática es un conjunto de dispositivos conectados entre sí para compartir información y recursos.

Por ejemplo, una red puede conectar computadoras, celulares, impresoras y otros dispositivos.

Internet es una enorme red mundial que conecta millones de dispositivos.`;

        }

        return `La Tecnología estudia herramientas, conocimientos y procesos utilizados para resolver problemas y satisfacer necesidades.

Actualmente incluye temas como programación, redes, inteligencia artificial, robótica, seguridad informática y desarrollo de aplicaciones.`;

    }


    // CIENCIAS

    if (subject === "Ciencias") {

        if (
            q.includes("fotosíntesis") ||
            q.includes("fotosintesis")
        ) {

            return `La fotosíntesis es el proceso mediante el cual las plantas producen su propio alimento.

Para realizarla utilizan principalmente:

• Luz solar
• Agua
• Dióxido de carbono

Como resultado producen glucosa y liberan oxígeno.

Este proceso es fundamental para la vida porque produce oxígeno y materia orgánica.`;

        }

        if (
            q.includes("célula") ||
            q.includes("celula")
        ) {

            return `La célula es la unidad básica de los seres vivos.

Existen dos grandes tipos:

• Células procariotas
• Células eucariotas

Las células eucariotas poseen un núcleo definido, mientras que las procariotas no tienen un núcleo rodeado por membrana.`;

        }

        return `Las Ciencias Naturales estudian diferentes aspectos de la naturaleza.

Entre sus áreas se encuentran la Biología, la Física, la Química y las Ciencias de la Tierra.

Para responder una pregunta científica es importante observar, formular hipótesis, analizar información y sacar conclusiones basadas en evidencias.`;

    }


    return "Elegí una materia para poder responder tu pregunta.";

}


// ==========================================
// MOSTRAR ERROR
// ==========================================

function showError(message) {

    errorMessage.textContent = message;

    errorMessage.style.display = "block";

}


// ==========================================
// OCULTAR ERROR
// ==========================================

function hideError() {

    errorMessage.style.display = "none";

}


// ==========================================
// HACER PREGUNTA
// ==========================================

askButton.addEventListener("click", function () {

    hideError();


    const selectedSubject = subject.value.trim();

    const userQuestion = question.value.trim();


    // VALIDACIÓN

    if (selectedSubject === "") {

        showError("⚠️ Primero tenés que seleccionar una materia.");

        subject.focus();

        return;
    }


    if (userQuestion === "") {

        showError("⚠️ Escribí una pregunta antes de continuar.");

        question.focus();

        return;
    }


    if (userQuestion.length < 5) {

        showError("⚠️ La pregunta es demasiado corta.");

        question.focus();

        return;
    }


    // CAMBIAR BOTÓN

    askButton.disabled = true;

    askButton.innerHTML = "⏳ Pensando...";


    // SIMULAR TIEMPO DE IA

    setTimeout(function () {

        const response = generateAnswer(
            selectedSubject,
            userQuestion
        );


        // MOSTRAR RESPUESTA

        answerSection.classList.remove("hidden");

        answerSubject.textContent = selectedSubject;

        answerText.textContent = response;


        // AGREGAR AL HISTORIAL

        addToHistory(
            selectedSubject,
            userQuestion,
            response
        );


        // RESTAURAR BOTÓN

        askButton.disabled = false;

        askButton.innerHTML = "🤖 Preguntar a StudyIA";


        // IR A RESPUESTA

        answerSection.scrollIntoView({
            behavior: "smooth"
        });


    }, 700);

});


// ==========================================
// HISTORIAL
// ==========================================

function addToHistory(subject, question, answer) {

    emptyHistory.style.display = "none";


    const item = document.createElement("div");

    item.className = "history-item";


    item.innerHTML = `

        <div class="history-question">

            ❓ ${escapeHTML(question)}

        </div>

        <div class="history-answer">

            🤖 ${escapeHTML(answer)}

        </div>

        <div class="history-subject">

            ${escapeHTML(subject)}

        </div>

    `;


    history.prepend(item);

}


// ==========================================
// PROTEGER HTML
// ==========================================

function escapeHTML(text) {

    const div = document.createElement("div");

    div.textContent = text;

    return div.innerHTML;

}


// ==========================================
// LIMPIAR HISTORIAL
// ==========================================

clearHistory.addEventListener("click", function () {

    const items = history.querySelectorAll(".history-item");


    if (items.length === 0) {

        return;

    }


    if (
        confirm("¿Querés borrar todo el historial?")
    ) {

        items.forEach(function (item) {

            item.remove();

        });


        emptyHistory.style.display = "block";

    }

});


// ==========================================
// MODO OSCURO
// ==========================================

themeButton.addEventListener("click", function () {

    document.body.classList.toggle("dark");


    if (
        document.body.classList.contains("dark")
    ) {

        themeButton.textContent = "☀️";

        localStorage.setItem(
            "studyia-theme",
            "dark"
        );

    } else {

        themeButton.textContent = "🌙";

        localStorage.setItem(
            "studyia-theme",
            "light"
        );

    }

});


// ==========================================
// RECORDAR TEMA
// ==========================================

const savedTheme =
    localStorage.getItem("studyia-theme");


if (savedTheme === "dark") {

    document.body.classList.add("dark");

    themeButton.textContent = "☀️";

}


// ==========================================
// BOTÓN RESUMIR
// ==========================================

summaryButton.addEventListener("click", function () {

    const currentAnswer = answerText.textContent;


    if (!currentAnswer) {

        return;

    }


    const sentences =
        currentAnswer
            .split(".")
            .filter(sentence => sentence.trim() !== "");


    if (sentences.length <= 2) {

        alert("La respuesta ya es bastante corta.");

        return;

    }


    const summary =
        sentences
            .slice(0, 2)
            .join(".") + ".";


    answerText.textContent =
        "📌 Resumen:\n\n" + summary;

});


// ==========================================
// ENTER + CTRL PARA ENVIAR
// ==========================================

question.addEventListener("keydown", function (event) {

    if (
        event.key === "Enter" &&
        event.ctrlKey
    ) {

        askButton.click();

    }

});
