function mostrarCategoria(categoria) {
    let produtos = {
        salgados: ["Coxinha", "Pastel", "Empada"],
        cafes: ["Expresso", "Cappuccino", "Mocha"],
        bebidas: ["Suco Natural", "Refrigerante", "Água de Coco"],
        refeicoes: ["Prato Executivo", "Marmitex", "Salada Especial"],
        sorvetes: ["Casquinha", "Sundae", "Milkshake"],
        acai: ["Açaí Puro", "Açaí com Banana", "Açaí com Leite Condensado"]
    };

    let conteudo = "<h3>" + categoria.charAt(0).toUpperCase() + categoria.slice(1) + "</h3><ul>";
    produtos[categoria].forEach(item => {
        conteudo += "<li>" + item + "</li>";
    });
    conteudo += "</ul>";

    document.getElementById("produtos").innerHTML = conteudo;
}
