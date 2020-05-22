<template>
  <div>
    <div>Modulo profesionales</div>
    <div v-for="especialidad in staff">
      <div class="servicio prof">
        <h2 class="uppercase green">{{especialidad.especialidad}}</h2>
        <div class="detalle">
          <div v-for="item in especialidad.profesionales">
            {{ item.name }}
            <span v-for="direccion in item.address">| {{ direccion }}</span>
            <span v-if="item.action">|</span>
            <a href="ingresar" title="turnos" v-if="item.action">Solicitar Turno</a>
            <div class="clear"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Profesionales",
  data: function() {
    return {
      staff: [
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "CARDIOLOGÍA ADULTOS",
          profesionales: [
            {
              name: "Dr. Brown, Luciano",
              address: ["San Luis 2176"],
              action: true
            },
            {
              name: "Dr. González, Horacio",
              address: ["Rawson 1774"],
              action: true
            },
            {
              name: "Dra. Petrucci, María Fernanda",
              address: ["San Luis 2176"],
              action: true
            },
            {
              name: "Dra.Ranchi, Rosana ",
              address: ["Av. Tejedor 264"],
              action: true
            }
          ]
        },
        {
          especialidad: "CARDIOLOGÍA PEDIÁTRICA",
          profesionales: [
            {
              name: "Dr. Andrés, Lucas",
              address: ["San Luis 2143"],
              action: true
            },
            {
              name: "Dr.Hozbor, Andrea",
              address: ["San Luis 2143", "San Luis 2453"],
              action: true
            }
          ]
        },
        {
          especialidad: "CIRUGÍA ADULTOS",
          profesionales: [
            {
              name: "Dr. Actis, Nicolás",
              address: ["San Luis 2176"],
              action: true
            }
          ]
        },
        {
          especialidad: "CIRUGÍA PEDIÁTRICA",
          profesionales: [
            {
              name: "Dr.Dramis, Matías ",
              address: ["San Luis 2143", "Av. Tejedor 264", "Garay 2239"],
              action: true
            },
            {
              name: "Dr.Kogan, Andrés ",
              address: ["San Luis 2143"],
              action: true
            },
            {
              name: "Dr. Yamahachi, Claudio",
              address: ["San Luis 2143"],
              action: true
            }
          ]
        },
        {
          especialidad: "CIRUGÍA PLÁSTICA	",
          profesionales: [
            {
              name: "Dra. Albarenque, Gabriela",
              address: ["Av. Tejedor 264"],
              action: true
            },
            {
              name: "Dr.Boix, Andrés ",
              address: ["San Luis 2176"],
              action: true
            },
            {
              name: "Dr.Parellada, Ernesto",
              address: ["Av. Tejedor 264"],
              action: true
            }
          ]
        },
        {
          especialidad: "CLÍNICA MÉDICA ADULTOS",
          profesionales: [
            {
              name: "Dr. Barretto, Mariano",
              address: ["San Luis 2143", "Av. Tejedor 264"],
              action: true
            },
            {
              name: "Dra. Rubiolo, Natalia",
              address: ["San Luis 2143"],
              action: true
            },
            {
              name: "Dra. Vezzozzi, Viviana",
              address: ["San Luis 2176"],
              action: true
            }
          ]
        },
        {
          especialidad: "DERMATOLOGÍA",
          profesionales: [
            {
              name: "Dra. Acosta, Marianela",
              address: ["San Luis 2176"],
              action: true
            },
            {
              name: "Dra. Stepa, Tatiana",
              address: ["San Luis 2176", "Av. Tejedor 264"],
              action: true
            }
          ]
        },
        {
          especialidad: "FONOAUDIOLOGÍA",
          profesionales: [
            {
              name: "Fga. Bauso, Carina	",
              address: ["San Luis 2176", "Av. Tejedor 264"],
              action: true
            },
            {
              name: "Fga. Canido Vallejos, Marcia	",
              address: ["San Luis 2176"],
              action: true
            }
          ]
        },
        {
          especialidad: "GASTROENTEROLOGÍA ADULTOS",
          profesionales: [
            {
              name: "Dr. Capriotti, Andrés",
              address: ["San Luis 2143"],
              action: true
            },
            {
              name: "Dr.Conosciutto, Juan Ignacio",
              address: ["San Luis 2143"],
              action: true
            },
            {
              name: "Dr.Rastelli, Laureano",
              address: ["San Luis 2143"],
              action: true
            }
          ]
        },
        {
          especialidad: "GINECOLOGÍA Y OBSTETRICIA",
          profesionales: [
            {
              name: "Dr.Amestoy, Julio",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dra.Carrión, Rocío",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Ilarregui, Ignacio",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Landi, Guillermo",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Lopez, Sebastián",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dra.Machado, Carmen",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dra.Mattioli, Susana",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Oddone, Fabrizio",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Pérez Staracci, Andrés",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Pirrotta, Néstor",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dra.Ponce Traverso, Jorgelina",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Quaglia, Horacio",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Rossini, Mariano",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Scafetto, Fabián",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dra.Segura, Agustina",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            },
            {
              name: "Dr.Simonetti, José",
              address: ["20 de Septiembre 1538", "Las Heras 3113"]
            }
          ]
        },
        {
          especialidad: "HEMATOLOGÍA",
          profesionales: [
            {
              name: "Dr.García, Carlos Alen",
              address: ["San Luis 2176"],
              action: true
            },
            {
              name: "Dr.García, Santiago Antuel",
              address: ["San Luis 2176", "Av. Tejedor 264"],
              action: true
            }
          ]
        },
        {
          especialidad: "INFECTOLOGÍA ADULTOS	",
          profesionales: [
            {
              name: "Dra. Bechini, Florencia	",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "INMUNOLOGÍA",
          profesionales: [
            {
              name: "Dr.Dr. Uriarte, Ignacio	",
              address: ["San Luis 2176"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        },
        {
          especialidad: "ANATOMÍA PATOLÓGICA",
          profesionales: [
            {
              name: "Dra. Maldonado Mariela",
              address: ["Av. Independecia 3650"],
              action: true
            }
          ]
        }
      ]
    };
  }
};
</script>

<style>
</style>
