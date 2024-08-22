<script>
export default {
    name: 'CardElon',
    data() {
        return {
            run: '22.222.222-2',
            apellidos: 'Jobs',
            nombres: 'Steven Paul',
            nacionalidad: 'Estadounidense',
            sexo: 'M',
            fNacimiento: '24/02/1955',
            nDocumento: '222.222.222',
            fEmision: '22/08/2024',
            fVencimiento: '22/08/2028'
        }
    }
}
</script>
<template>
    <div class="carnet">
        <aside>
            <div>
                <span>CEDULA DE INDENTIDAD</span>
                <img width="40" src="../assets/chile_bandera.png" alt="Bandera Chilena" />
            </div>

            <img src="../assets/foto_steve.jpg" alt="Steve Jobs Foto Carnet" />
            <p>RUN {{ run }}</p>
        </aside>

        <main>
            <header>
                <p>REPUBLICA DE CHILE</p>
                <span>SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN</span>
            </header>
            <section>
                <article>
                    <header>APELLIDOS</header>
                    <span>{{ apellidos }}</span>
                </article>
                <article>
                    <header>NOMBRES</header>
                    <span>{{ nombres }}</span>
                </article>

                <div class="grid-2-colums">
                    <article>
                        <header>NACIONALIDAD</header>
                        <span>{{ nacionalidad }}</span>
                    </article>
                    <article>
                        <header>SEXO</header>
                        <span>{{ sexo }}</span>
                    </article>
                </div>
                <div class="grid-2-colums">
                    <article>
                        <header>FECHA DE NACIMIENTO</header>
                        <span>{{ fNacimiento }}</span>
                    </article>
                    <article>
                        <header>NÙMERO DOCUMENTO</header>
                        <span>{{ nDocumento }}</span>
                    </article>
                </div>
                <div class="grid-2-colums">
                    <article>
                        <header>FECHA DE EMISIÓN</header>
                        <span>{{ fEmision }}</span>
                    </article>
                    <article>
                        <header>FECHA DE VENCIMIENTO</header>
                        <span>{{ fVencimiento }}</span>
                    </article>
                </div>
                <article>
                    <header>FIRMA DEL TITULAR</header>
                    <span>steven jobs</span>
                </article>
            </section>
        </main>
    </div>
</template>
<style scoped>
.carnet {
    width: 400px;
    height: 230px;
    background: #c8deed;
    border-radius: 20px;
    display: grid;
    grid-template-columns: 30% 1fr;
    padding: 15px;
    box-shadow: 0px 0px 10px 2px black;
}

aside div {
    display: flex;
}

aside>img {
    margin-top: 15px;
    width: 100%;
}

aside p {
    text-align: center;
    font-size: 12px;
    font-weight: bold;
}

main {
    padding: 0px 14px;
}

main article {
    margin: 4px 0px;
}

main article header {
    font-weight: bold;
    color: #0235a4;
    font-size: 8px;
}

main header p {
    font-size: 20px;
    margin: 0;
    font-weight: bold;
    color: #0235a4;
}

main header span {
    font-size: 8px;
    color: #399be1;
}

main section {
    margin-top: 10px;
}

main section article span {
    font-size: 13px;
    font-weight: 600;
}

main section .grid-2-colums {
    display: grid;
    grid-template-columns: 50% 50%;
}
</style>