<template>
    <div class="modelo">
        <h2 class="nuestros text-right p-0 col-md-6 col-lg-4 col-11" style=" font-family: 'Kollektif';">NUESTRO MODELO</h2>
        <div class="row cont-A justify-content-center pad-paciente align-items-center">
            <div class=" borde-paciene-uno col-md-6">
                <h1 class="texto-paciente texto-paciente-uno text-right " style="font-family: 'Kollektif'; letter-spacing: 5px;">1.</h1>
                <h3 class="texto-paciente-uno item-paciente text-right " style="font-family: 'Kollektif'; letter-spacing: 5px;">Contáctate<br/> con nosotros</h3>
            </div>
            <div data-aos="zoom-out" class=" col-md-6  m-0 row justify-content-center align-items-center">
                <img src="@/assets/modelo/1.png" alt="" class="img-model-T">
            </div>
        </div>
        <div class="row cont-B justify-content-center pad-paciente align-items-md-center flex-lg-row flex-md-row flex-column-reverse">
             <div data-aos="zoom-out" class=" col-md-6 m-0 row justify-content-center align-items-center">
                <img src="@/assets/modelo/2.png" alt="" class="img-model">
            </div>

            <div class=" borde-paciene-dos mb-4 col-md-6">
                <h1 class="texto-paciente texto-paciente-dos text-left " style="font-family: 'Kollektif'; letter-spacing: 5px;">2.</h1>
                <h3 class="texto-paciente-dos item-paciente text-left " style="font-family: 'Kollektif'; letter-spacing: 5px;">Afíliate a<br/> nuestros beneficios</h3>
            </div>
        </div>
        <div class="row cont-A justify-content-center pad-paciente align-items-md-center">
            <div class="borde-paciene-tres col-md-6 mb-4">
                <h1 class="texto-paciente texto-paciente-tres text-right" style="font-family: 'Kollektif'; letter-spacing: 5px;">3.</h1>
                <h3 class="texto-paciente-tres item-paciente text-right" style="font-family: 'Kollektif'; letter-spacing: 5px;">Elige la ortopedia<br/> de tu interés</h3>
            </div>
            <div data-aos="zoom-out" class="col-md-6 m-0 row justify-content-center align-items-center">
                <img src="@/assets/modelo/3.png" alt="" class="img-model-D">
            </div>
        </div>
        <div class="row cont-B justify-content-center pad-paciente align-items-md-center flex-lg-row flex-md-row flex-column-reverse">
             <div data-aos="zoom-out" class=" col-md-6 m-0 row justify-content-center align-items-center">
               <img src="@/assets/modelo/4.png" alt="" class="img-model">
            </div>

            <div class="borde-paciene-cuatro col-md-6">
                <h1 class="texto-paciente texto-paciente-cuatro text-left " style="font-family: 'Kollektif'; letter-spacing: 5px;">4.</h1>
                <h3 class="texto-paciente-cuatro item-paciente text-left " style="font-family: 'Kollektif'; letter-spacing: 5px;">Disfruta de nuestros <br/> beneficios sin preocupaciones</h3>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'NuestroModelo'
}
</script>
<style>
.bc8b006f-41d7-45b7-9b45-b7ac5824b26a{
    fill:none;
    }
.ea1ac8ee-0e9c-4747-9420-16c3a80e21a3{
    fill:#dfdfdf;
    }
.bd5a03fa-29b4-436b-a84b-43f458d735c2{
    fill:#2e353b;
    }
.b396b990-c08d-4f94-aa64-b02afe0aa8f1{
    fill:#fafafa;
    }
.a037c674-fb0b-4f4b-91c3-64644be5730b{
    opacity:0.2;
    }
.a8c60437-e27a-4e99-9e4e-9d5e04da1758{
    clip-path:url(#b7a59301-65ca-488e-9896-11fedbde208c);
    }
.a3a51133-1983-433b-bdab-1091fb26bc7d{
    fill:#d8986c;
    }
.f29ac1c6-86e9-424b-a8fa-a6bd5aaf75dd{
    fill:#4d5a64;
    }
.ffc1ecfd-44d5-41c1-81e0-a9cc83b349d9{
    fill:#c97544;
    }
.bede9584-758b-471e-aad1-054fce723726{
    fill:#0d0006;
    }
.paciente{
    width: 20rem;
}
.pacienteD{
    width: 28rem;
}
.texto-paciente{
    font-size: 10rem;
    font-family: 'Roboto';
}
.texto-paciente-uno{
    color: #DD3B00;
    margin-left: 1rem;
    margin-right:1rem;
}
.item-paciente{
    font-size: 3rem;
    font-family: 'Roboto';
}
.borde-paciene-uno{
    border-right: solid 1rem #DD3B00;
    height: 30rem;
    margin-right: -1rem;
}
.texto-paciente-dos{
    color: #2359E5;
    margin-left: 1rem;
    margin-right:1rem;
}
.borde-paciene-dos{
    border-left: solid 1rem #2359E5;
    height: 30rem;
    margin-left: -1rem;
}

.texto-paciente-tres{
    color: #F7E200;
    margin-left: 1rem;
    margin-right:1rem;
}
.borde-paciene-tres{
    border-right: solid 1rem #F7E200;
    height: 30rem;
    margin-right: -1rem;
}

.texto-paciente-cuatro{
    color: #66B42B;
    margin-left: 1rem;
    margin-right:1rem;
}
.borde-paciene-cuatro{
    border-left: solid 1rem #66B42B;
    height: 30rem;
    margin-left: -1rem;
}
.modelo{
    margin-bottom: 12rem;
}

.pad-paciente{
    padding: 3rem;
}
.img-model{
    width: 100%
}
.img-model-D{
    width: 90%
}
.img-model-T{
    width: 73%
}
.cont-A{
    max-width: 100%;
    margin-left: auto!important;
    margin-right: 0!important
}
.cont-B{
    max-width: 100%;
    margin-right: auto!important;
    margin-left: 0!important;
}
@media only screen and (max-width: 600px){ 
    .paciente {
        width: 17rem;
        margin-top:2rem; 
    }
    .pacienteD{
        width: 17rem;
    }
    .pad-paciente {
        padding: 1rem;
    }
    .borde-paciene-uno {
        border-right: solid 0.5rem #DD3B00;
         margin-left: 0rem; 
             height: 12rem;
    }
    .borde-paciene-dos{
        border-left: solid 0.5rem #2359E5;
        margin-right:4rem;
            height: 12rem;
    }

    .borde-paciene-tres{
        border-right: solid 0.5rem #F7E200;
        margin-left: -5rem;
            height: 12rem;
    }

    .borde-paciene-cuatro{
        border-left: solid 0.5rem #66B42B;
        margin-right:4rem;
            height: 14rem;
    }
    .img-model{
        margin-top:2rem
    }
      .item-paciente {
        font-size: 1.6rem;
        font-family: 'Roboto';
    }
    .pad-paciente {
        padding: 0rem 3rem 3rem 3rem;
    }
    .texto-paciente {
        font-size: 5rem;
        font-family: 'Roboto';
    }
    .texto-paciente-uno{
    color: #DD3B00;
    margin-left: 0.5rem;
    margin-right:0.5rem;
}
.texto-paciente-dos{
    color: #2359E5;
    margin-left: 0.5rem;
    margin-right:0.5rem;
}
.texto-paciente-tres{
    color: #F7E200;
    margin-left: 0.5rem;
    margin-right:0.5rem;
}
.texto-paciente-cuatro{
    color: #66B42B;
    margin-left: 0.5rem;
    margin-right:0.5rem;
}
.img-model{
    width: 30rem
}
.img-model-D{
    width: 25rem
}
.img-model-T{
    width: 25rem
}
}
@media only screen and (max-width: 768px) {
    .paciente {
        width: 17rem;
        margin-top:2rem;
    }
    .pacienteD{
        width: 17rem;
    }
    .item-paciente {
        font-size: 1.6rem;
        font-family: 'Roboto';
    }
    .pad-paciente {
        padding: 0rem 3rem 3rem 3rem;
    }
    .texto-paciente {
        font-size: 5rem;
        font-family: 'Roboto';
    }
}
@media only screen and (max-width: 1024px) and (min-width: 769px){
    .paciente {
        width: 16rem;
        margin-top: 2rem;
    }
    .item-paciente {
        font-size: 2rem;
        font-family: 'Roboto';
    }
    .texto-paciente {
        font-size: 7rem;
        font-family: 'Roboto';
    }
    .pad-paciente {
        padding: 0rem 3rem 3rem 3rem;
    }
    
  
}

.b46370da-5188-4cd3-a258-46d4c884c7b6{
    fill:none;
}
.b979ca66-c55e-4f2f-8ab0-73248733b3f8{
    fill:#37240c;
}
.eee5f2ec-3a79-4b1a-87dc-82f5a95ac3ac{
    fill:#797979;
}.f85f44f1-eb57-435d-9ebd-0ea91706854d{
    fill:#8d5d14;
}
.afd3556d-b2de-40f7-a29a-995ec4c16499{
    fill:#dfdfdf;
}.ac350edd-43a1-4f1c-8204-87f28100e811{
    fill:#d8986c;
}
.ae0b7b62-218f-4109-9600-bccff333761c{
    fill:#263d13;
}.f111c3c4-2104-4f4b-9332-8ff6b5743b07{
    fill:#0d0006;
}
.b4a1718f-42a4-49aa-a61e-ae9645a062df{
    fill:#5e3a08;
}.e864e1a4-591f-41b3-860c-a245cf918f13{
    fill:#a69d63;
}
.ad76b368-6395-482f-a888-bf6817ab5820{
    fill:url(#fe5-0cdb-413a-9ace-70cbf93332d9);
}.e005794f-0a50-4455-807d-b0286a2a0371{
    fill:#fff;
}
.e2a12528-c884-44ec-8852-2eb96cea3b3d{
    fill:url(#b816c48a-2179-422a-80bf-e9a1f7be615d);
}.b2927917-61d3-4779-9070-d0323c94beda{
    fill:url(#a9955c24-396f-488b-b46b-b9ace3f76cef);
}.b0cde138-8c4d-4516-95b2-24ebc83a5169{
    fill:url(#a5fdd278-d3a5-4689-841b-ba9e7ea9139a);
}.b440810a-ab12-4bac-802d-6514e6dbd7c7{
    fill:url(#f925fd92-1378-434f-8810-5de15ec604ac);
}.ad103272-1fad-4c95-9d1e-a9743114d8a4{
    fill:url(#f841576a-34a5-4369-aa26-268ee71f2eb9);
}.b313362b-baeb-4eb0-b893-a181bbba5732{
    opacity:0.58;
}.b721f7be-5b15-49db-8f38-9b56c0a66e02{
    clip-path:url(#b3b1005d-c2ba-4713-8900-18111af46fe8);
}.ad1676fb-31d1-4e5d-9b65-9f9c779f7761{
    fill:url(#ed4e898c-37f6-48d3-ad3d-8314e4608c9b);
}.a88771d8-ce02-4b0f-8910-20e53c7111a3{
    fill:url(#be2f926c-c99c-413c-8d2a-93f4ad6ce840);
}.aab29596-feed-4157-95ff-2f4cb5d51582{
    fill:url(#fee0b94c-2059-4917-9788-f0f6cbb20a52);
}.b758c610-0876-4e86-953d-afedae49c442{
    fill:#1a260f;
}.a98f5c7f-2cd0-49a4-885e-d8af98a50bd7{
    fill:#9a9a9a;
}.a2807c56-1e0b-45f6-af51-b633ca9865c2{
    fill:#2e353b;
}.ecce9d2d-1eac-4858-afbd-c995c38d7120{
    fill:#212528;
}.bd2bf375-9e6e-4f93-97eb-8d14a4171a4a{
    fill:#c97544;
}.ae8ef3df-f9f8-417a-b1da-6befc5342d04{
    fill:#fafafa;
}
.aaf04770-2b59-467b-a247-56387d222b4d,.af1e460b-854d-452a-89d2-7e1eb47f8e8c,.fc51fb53-29be-4d60-8621-b33f393ace0b{
    fill:none;
}
.fc503775-1b1f-4706-814b-dd6188de34fe{
    isolation:isolate;
}
.b3533b50-9f73-4110-9bf2-ca77defdb931{
    fill:#8d5d14;
}
.e2157c75-1bd7-432c-b995-f2dc09cf2b7a{
    fill:#dfdfdf;
}
.a46e5965-a0e6-4254-96ee-244a7c19bba7{
    clip-path:url(#a9de9778-5add-406a-8b14-f4860a6b6e39);
}
.b087bda5-f52b-4957-a9e3-9a10cc3a8b9b{
    fill:url(#b6c77ea8-ad59-4967-80b1-82b9e0b8ae46);
}
.beb7d72e-230e-4f82-b30d-a9d138fffaae{
    clip-path:url(#b7040c0b-d461-4664-87f2-12d072eee269);
}.ed9ee9a1-dd03-4fc7-8276-bc9bfe9d546a{
    fill:url(#f345f63d-8685-4bad-b7c5-76a071751119);
}
.bf669048-f427-46e6-b045-c6e1f0fd2d5e{
    fill:#d8986c;
}
.b0433bd3-1fdf-4b30-8343-b44bba2791c6{
    fill:#9a9a9a;
}
.a819c739-1293-4ccb-af3c-ea46d6b39fe5{
    fill:#191c26;
}
.e459015d-62f9-42b6-9c8e-a21794e3bc9c{
    fill:#e99b6b;
}.b52566ae-83c9-450f-93c3-75cf5d35f7fa{
    fill:#e6877d;
}.f4fd6de7-7925-4104-ac16-3c06706d73ad{
    fill:#c97544;
}.fd4a4c15-2337-4180-addf-6f8d192ceca1{
    opacity:0.45;
}.aa10f311-2d59-47d2-81b9-f46c1e588f84{
    clip-path:url(#e1bf85db-0862-447f-90e6-e8593b061c2d);
}
.fa0ef7f0-e227-491d-a6aa-14106a4fefaf{
    fill:#f3cbad;
}
.a7d1fc63-b49c-4ba1-becc-ff0e929ded1a{
    fill:#dd956a;
}
.a7a8e20a-951c-41be-9cec-7bc7a4cce42a{
    fill:#212528;
}
.bdfa60c5-fa61-43b0-9b4e-49279e4d84c2{
    fill:#e57f4e;
}
.fcd7d488-7f7a-4bc3-bcc4-432a3dbd6b5b{
    fill:#e68673;
}
.f808e1fa-dfd2-49f4-b509-85e6305515c6{
    fill:#f7f4ea;
}
.b4c30a7d-3146-4b0e-9cf3-f4d9253db135{
    fill:#bc6657;
}
.a30daf79-ac75-44aa-96f4-6b767ed06f0e{
    fill:#fff;
}
.e01a1605-00a7-46c5-922d-f4df8ee5241c{
    fill:#2e2e45;
}
.af1e460b-854d-452a-89d2-7e1eb47f8e8c{
    stroke:#fff;stroke-linejoin:round;stroke-width:0.87px;
}
.aaf04770-2b59-467b-a247-56387d222b4d,.af1e460b-854d-452a-89d2-7e1eb47f8e8c{
    stroke-linecap:round;
}
.f0e5e3b2-dcf5-49e4-918a-e9d32c57cdfa{
    fill:#72a8f7;
}
.bdda74cf-3e65-43ed-ba03-dc7bb12129f0{
    mix-blend-mode:multiply;
}
.bf9a5da6-6561-4616-bdeb-971c19ab8761{
    clip-path:url(#bc21c04e-e8e4-44cd-ace4-d270adae087f);
}.a872a039-cc42-4968-a71a-dd102e463067{
    fill:#f2f2f2;
}.f5ab5138-d462-466d-8709-aee4d0bb06e0{
    fill:#3f4f80;
}.b808b581-35aa-4e0f-82d5-2cd19ca4bdc1{
    fill:#c4c6d3;
}.a4075492-7295-4052-8e66-79896eeeb4fb{
    fill:#1c1d3e;
}
.b8332f42-0260-4ef6-a028-29ca33451574{
    fill:#333a50;
}
.acaab02c-4f56-4e23-a5be-64a4a4e6b603{
    fill:#272f45;
}
.bf93b591-78c4-4256-be43-edccdd83c71e{
    fill:#0d0006;
}
.b79b5db3-a65f-4dd8-bb7a-be4caf49765c{
    fill:#2e353b;
}
.aaf04770-2b59-467b-a247-56387d222b4d{
    stroke:#c97544;stroke-miterlimit:10;stroke-width:0.25px;
}
.a3d7ec18-0a71-4ef4-a28d-32b36902dc3f{
    fill:#fafafa;
}
.a48fbd20-7f2f-4f27-ba26-5cc20cfe6d01,.a820ed4f-d28c-48a9-aae6-34af1d27bc8b,.a8757bb3-6a3f-482a-91ab-26bc7e44c97d,.a91a4db1-49c5-415e-9fb3-5657bb6e486b,.ab245332-4d44-4ed5-9d17-44ebbd20dae0,.ad2092b5-1a6d-431c-ae0c-49eee391039b,.ada65f7c-68f5-43a1-b897-686db21c9c23,.b63c9386-6d73-4b28-a77e-54362825b998,.b7642690-0d37-49dd-a058-9e761667a559,.b7d695f9-e593-4070-aef7-8c3b9bc45e1c,.b93aadfb-f58e-4aed-bdba-dc387a28908f,.b9a17859-ca59-49d0-a2b4-8e32de776593,.bb424537-200b-494a-8345-4b6375492679,.bc4fb77f-ffba-4137-a191-b9db3815aeb6,.be36a83d-506b-46f5-aa2c-38e86d225de6,.e5cdd3b6-846c-452b-a58d-ceb11c7a6426,.e88eb903-921c-4e51-8ac0-4cd197cd31b6,.ec089139-d8b1-4d1d-a7be-f3a6f79a09a9,.edeb5442-7528-4c3e-b77f-37f9b9e4843f,.f5a4f138-8598-44de-9fb3-a348d1981a8e,.f63b1d51-c3c1-4624-9d17-9da01428dd72,.f99fb052-ef54-4fb6-8e39-57c54e74c2b8{
    fill:none;
}.a9f1c3c6-2a79-40e6-a0c8-a70824ba98e0{
    fill:#b7e8f4;
}
.a11577b2-364c-43f8-bf9e-f181b9a8f7b4,.f2a1c666-8668-401b-8fcc-118e053df5cf{
    fill:#000016;
}
.a11577b2-364c-43f8-bf9e-f181b9a8f7b4,.a50388f2-d6f7-4f10-849f-cb203666cd26,.a64ff5e6-a69d-4862-81c6-724a8dc7ca4a,.a7bce75c-9f2a-4baa-8e94-533e3d89e9b8,.ab035c50-0561-4087-abc4-36003a6309d5,.aeb3a0b5-f1bf-42df-8095-3dc56bd19c2a,.b4c4d2b9-40af-4cc7-a753-7e02d872cfc8,.bfc64001-876f-43a0-8427-93d0959bb841,.e58c083e-6b4e-4082-9e20-21cdaeba7a27,.e8926de7-3158-4b84-90ef-8bf8efb6e0b3,.e8cab13d-c592-4eef-b2e8-1dfa9a6fbaa3,.ead8ce2c-bcff-4302-871f-4c4b3d84987d,.eb0e396b-9319-40f9-a31b-4f00dd37ccc7,.f328ecce-445b-4d3f-ac6b-8e4c9dd933bd,.f3a16397-ecc4-4687-8a3b-f9b5e7f321e4,.f9907326-c23d-4a87-a55b-d956bc1c89b5{
    fill-rule:evenodd;
}
.a64ff5e6-a69d-4862-81c6-724a8dc7ca4a{
    fill:#3e415f;
}
.ab035c50-0561-4087-abc4-36003a6309d5{
    fill:#181b3a;
}
.b5149304-6463-4042-a60e-74694d96646e{
    fill:#464646;
}.b4706f88-f37b-4256-b586-f40c4f215dcf{
    fill:#c3eef9;
}
.b24e5b0d-26cf-4269-af1f-ecc4334b0890{
    fill:#eefa94;
}
.aacc8fc4-5f97-433a-a169-5de2d1b3f49b{
    fill:#e09897;
}
.eb076401-9f7b-4385-8dfa-2566e3ad6631{
    fill:#dfb368;
}
.a58ff421-a02c-4b57-9fb3-55e939ed894c{
    fill:#b6f390;
}
.a3658c53-a0cd-441f-917e-05a963ac9cd6,.aeb3a0b5-f1bf-42df-8095-3dc56bd19c2a{
    fill:#fff;
}
.b4c4d2b9-40af-4cc7-a753-7e02d872cfc8,.b5015e43-c417-43c8-af03-938d48203a44{
    fill:#e2e0e7;
}
.e8cab13d-c592-4eef-b2e8-1dfa9a6fbaa3{fill:#bc4c45;}.b85549d6-554a-48d8-81a7-29bbcaee4e78,.eb0e396b-9319-40f9-a31b-4f00dd37ccc7{
    fill:#0f0e29;
}
.a7bce75c-9f2a-4baa-8e94-533e3d89e9b8{
    fill:#c3864f;
}
.e58c083e-6b4e-4082-9e20-21cdaeba7a27{
    fill:#a46b41;
}
.b9c90227-258f-4774-a019-34a911c07936{
    fill:#def5fc;
}
.f679b0b3-6109-46b7-a1f1-5474fe63c2cd{
    fill:#d8986c;
}
.a7b8fb0a-371a-49b5-abf4-eafc568eea99{
    fill:#868686;
}
.b2170c81-672a-4f06-9f9c-e7cdc21bb547{
    fill:#ebeceb;
}
.bbd58538-509f-46a2-b615-207b05ea6b7d{
    fill:#393663;
}.f6857485-029a-475b-a6f5-2860ff36806d{
    fill:#7bb8f8;
}.b93aadfb-f58e-4aed-bdba-dc387a28908f{
    stroke:#393663;stroke-width:0.5px;
}
.a820ed4f-d28c-48a9-aae6-34af1d27bc8b,.a8757bb3-6a3f-482a-91ab-26bc7e44c97d,.b93aadfb-f58e-4aed-bdba-dc387a28908f,.be36a83d-506b-46f5-aa2c-38e86d225de6,.e5cdd3b6-846c-452b-a58d-ceb11c7a6426{
    stroke-miterlimit:10;
}
.bdad0908-5520-42a8-966a-6ad0dd425037{
    fill:#dc5851;
}
.ef85bd94-e6c8-44f4-a0dc-6c864f8e7932{
    fill:#dfcbb5;
}
.e6c6880d-e2ec-46cb-ae8c-30abfe582ed2{
    fill:#0d0006;
}
.a2854795-6b33-4826-af64-b819a045e43a{
    fill:#2e353b;
}
.b4fd99b5-912c-47fa-97f3-090b37f8078e{
    fill:#b9b9ba;
}
.f1c55304-791b-4669-b6b5-8245d70b8770{
    fill:#0000a8;
}
.a820ed4f-d28c-48a9-aae6-34af1d27bc8b{
    stroke:#00005b;stroke-width:0.25px;
}
.f90eb95c-a480-4b34-baad-914c9a675ec8{
    fill:#c97544;
}
.be36a83d-506b-46f5-aa2c-38e86d225de6{
    stroke:#a9a9a9;stroke-width:9px;
}
.a48fbd20-7f2f-4f27-ba26-5cc20cfe6d01,.a91a4db1-49c5-415e-9fb3-5657bb6e486b,.ab245332-4d44-4ed5-9d17-44ebbd20dae0,.ad2092b5-1a6d-431c-ae0c-49eee391039b,.ada65f7c-68f5-43a1-b897-686db21c9c23,.b63c9386-6d73-4b28-a77e-54362825b998,.b7642690-0d37-49dd-a058-9e761667a559,.b7d695f9-e593-4070-aef7-8c3b9bc45e1c,.b9a17859-ca59-49d0-a2b4-8e32de776593,.bb424537-200b-494a-8345-4b6375492679,.bc4fb77f-ffba-4137-a191-b9db3815aeb6,.be36a83d-506b-46f5-aa2c-38e86d225de6,.e88eb903-921c-4e51-8ac0-4cd197cd31b6,.ec089139-d8b1-4d1d-a7be-f3a6f79a09a9,.edeb5442-7528-4c3e-b77f-37f9b9e4843f,.f5a4f138-8598-44de-9fb3-a348d1981a8e,.f63b1d51-c3c1-4624-9d17-9da01428dd72{
    stroke-linecap:round;
}
.addc7d47-af30-4959-8dde-23220b34894f{
    fill:#edcbf8;
}
.afa58fb6-3edd-4cf4-8517-4cd8a7b71171{
    fill:#cf7c6a;
}
.e36b7b50-4e33-4527-a8fb-9946cf77b7fa{
    fill:#0f0f0f;
}
.bb39b8b2-a15d-42c2-90c6-f30eb9af84c7{
    clip-path:url(#fa245d8c-c17f-4153-92dd-ff619dce49ec);
}
.a5466a61-004d-4e1e-ac5f-e2c29404c604{
    fill:#db4200;
}
.a577b2b1-7f3f-4c3e-adfb-ce8827e24ddf{
    clip-path:url(#fa18e337-1974-4fdc-ab31-5870d69b31e2);
}
.ab245332-4d44-4ed5-9d17-44ebbd20dae0,.ada65f7c-68f5-43a1-b897-686db21c9c23,.b63c9386-6d73-4b28-a77e-54362825b998,.bb424537-200b-494a-8345-4b6375492679,.f63b1d51-c3c1-4624-9d17-9da01428dd72{
    stroke:#000;
}
.a48fbd20-7f2f-4f27-ba26-5cc20cfe6d01,.a91a4db1-49c5-415e-9fb3-5657bb6e486b,.ab245332-4d44-4ed5-9d17-44ebbd20dae0,.ad2092b5-1a6d-431c-ae0c-49eee391039b,.ada65f7c-68f5-43a1-b897-686db21c9c23,.b63c9386-6d73-4b28-a77e-54362825b998,.b7642690-0d37-49dd-a058-9e761667a559,.b7d695f9-e593-4070-aef7-8c3b9bc45e1c,.b9a17859-ca59-49d0-a2b4-8e32de776593,.bb424537-200b-494a-8345-4b6375492679,.bc4fb77f-ffba-4137-a191-b9db3815aeb6,.e88eb903-921c-4e51-8ac0-4cd197cd31b6,.ec089139-d8b1-4d1d-a7be-f3a6f79a09a9,.edeb5442-7528-4c3e-b77f-37f9b9e4843f,.f5a4f138-8598-44de-9fb3-a348d1981a8e,.f63b1d51-c3c1-4624-9d17-9da01428dd72{
    stroke-linejoin:round;
}
.ab245332-4d44-4ed5-9d17-44ebbd20dae0,.ad2092b5-1a6d-431c-ae0c-49eee391039b{
    stroke-width:0.95px;
}
.b3b191e2-0a23-434f-9a00-a84bfd048bd4{fill:#de9889;}.a48fbd20-7f2f-4f27-ba26-5cc20cfe6d01,.b7d695f9-e593-4070-aef7-8c3b9bc45e1c,.ec089139-d8b1-4d1d-a7be-f3a6f79a09a9{
    stroke:#c57266;
}
.a48fbd20-7f2f-4f27-ba26-5cc20cfe6d01{
    stroke-width:0.75px;
}
.b1ff00a7-9e1d-4342-9446-e6375ace9109{
    fill:#262722;
}
.e30cc9df-b455-4720-8284-25acf70df787{
    fill:#1e0a00;
}
.ada65f7c-68f5-43a1-b897-686db21c9c23,.b7d695f9-e593-4070-aef7-8c3b9bc45e1c{
    stroke-width:0.69px;
}
.adf09b80-770f-41bf-ace5-bae799a43760{
    fill:#7893fd;
}
.a91a4db1-49c5-415e-9fb3-5657bb6e486b{
    stroke:#5d7dec;stroke-width:0.67px;
}
.e384b91c-5b68-47cd-affa-a2300b35c9bc{
    fill:#c67d66;
}
.b9a17859-ca59-49d0-a2b4-8e32de776593{
    stroke:#a9523b;stroke-width:0.75px;
}
.bef7a620-27a3-4789-a9d0-9a0508c1fc5f{
    clip-path:url(#e7b69ac6-a871-470c-9b4a-6873fbc732af);
}
.a996e62e-c07a-4124-8232-471a9cba2e0a{
    clip-path:url(#b853a088-ffb0-40b6-b771-31eee7ec8237);
}
.a998d54e-9e3c-4178-9631-18d0890d059f{
    fill:#9fb6fd;
}
.abcd64c1-893d-4580-8e67-7644d4bb4572{
    fill:#e17d9f;
}
.f305370f-e986-4401-ba83-60393b5423cc{
    fill:#a84b16;
}
.b7642690-0d37-49dd-a058-9e761667a559{
    stroke:#4b8885;
}
.b7642690-0d37-49dd-a058-9e761667a559,.e5cdd3b6-846c-452b-a58d-ceb11c7a6426{
    stroke-width:1.94px;
}
.a2bd049f-fc55-42d6-924c-95cb60a2ebdc{
    fill:#e7a89d;
}
.b595f5bc-4e8d-483f-a991-b6cdc10ca93c{
    fill:#4b8885;
}
.ec768a47-fb0e-4cdf-9a51-97a98c6a3ed3{
    fill:#a38071;
}.ec089139-d8b1-4d1d-a7be-f3a6f79a09a9{
    stroke-width:0.69px;
}
.f7b359e8-8c2b-4974-99ec-91930b672977{
    fill:#eec863;
}
.a8757bb3-6a3f-482a-91ab-26bc7e44c97d,.e5cdd3b6-846c-452b-a58d-ceb11c7a6426{
    stroke:#fff;
}
.b570f085-501d-4747-871a-b9fbb09f7853{
    fill:#e8b395;
}
.ad2092b5-1a6d-431c-ae0c-49eee391039b{
    stroke:#484848;
}
.f5a4f138-8598-44de-9fb3-a348d1981a8e{
    stroke:#1e0a00;stroke-width:0.96px;
}
.fc4143a1-a283-44a0-9b84-6303a1b4b5fa{
    opacity:0.23;
}
.b1bcc014-14e4-4a79-afbd-e604b43968ab{
    clip-path:url(#f5085e9e-f2ca-4d0c-8086-080f0444f549);
}
.fe213323-c27b-49de-a799-fe5ae6643370{
    clip-path:url(#b384c570-fa29-4e4a-ad95-ec4a0a9279c9);
}
.a8757bb3-6a3f-482a-91ab-26bc7e44c97d{
    stroke-width:0.49px;
}
.bf1d8616-3f92-48e1-b341-b4baf32785a1{
    fill:#e9af90;
}
.b63c9386-6d73-4b28-a77e-54362825b998{
    stroke-width:0.92px;
}
.bc4fb77f-ffba-4137-a191-b9db3815aeb6{
    stroke:#d5668e;stroke-width:0.95px;
}
.a6511471-4dc6-48a6-8fed-0b1f7090de90{
    fill:#e1a78b;
}
.f63b1d51-c3c1-4624-9d17-9da01428dd72{
    stroke-width:0.87px;
}
.e88eb903-921c-4e51-8ac0-4cd197cd31b6,.edeb5442-7528-4c3e-b77f-37f9b9e4843f{
    stroke:#b9625c;
}
.edeb5442-7528-4c3e-b77f-37f9b9e4843f{
    stroke-width:0.64px;
}
.bb424537-200b-494a-8345-4b6375492679,.e88eb903-921c-4e51-8ac0-4cd197cd31b6{
    stroke-width:0.66px;
}
.bfc64001-876f-43a0-8427-93d0959bb841{fill:#aca9b8;
}
.f9907326-c23d-4a87-a55b-d956bc1c89b5{
    fill:#d5775f;
}
.a50388f2-d6f7-4f10-849f-cb203666cd26{
    fill:#e4ab81;
}
.e8926de7-3158-4b84-90ef-8bf8efb6e0b3{
    fill:#1f223d;
}
.f328ecce-445b-4d3f-ac6b-8e4c9dd933bd{
    fill:#db8900;
}
.ead8ce2c-bcff-4302-871f-4c4b3d84987d{
    fill:#eec100;
}
.f3a16397-ecc4-4687-8a3b-f9b5e7f321e4{fill:#707285;
}

</style>