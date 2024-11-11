/**
 * JS Jokenpo
 * @author Caio Lopes
 */

function jogar() {
    if (document.getElementById("pedra").checked == false && document.getElementById("papel").checked == false && document.getElementById("tesoura").checked == false) {
        alert("Selecione uma opção");
    } else {
        //Lógica principal
        var sorteio = math.floor(Math.random() * 3)
        switch (sorteio) {
            case 0:
                document.getElementById(monitor).src = "pcpedra"
                break
            case 1:
                document.getElementById(monitor).src = "pcpapel"
                break
            case 2:
                document.getElementById(monitor).src = "pctesoura"
                break
        }
    }
}

function resetar() {
    document.getElementById("monitor").src = "monitor.png"
    document.getElementById("placar").innerHTML = ""
}
