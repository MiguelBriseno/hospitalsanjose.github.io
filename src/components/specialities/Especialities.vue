<template>
    <div class="bg-white py-24 sm:py-32">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
            <div class="mx-auto max-w-4xl text-center">
                <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">NUESTRAS ESPECIALIDADES</h2>
                <p class="mt-6 text-lg leading-9 text-gray-600 text-justify">Descubre nuestra amplia gama de especialidades en oftalmología, diseñadas para brindarte el mejor cuidado visual. Desde tratamientos avanzados hasta cirugías de vanguardia, nuestro equipo de expertos está comprometido con proteger y mejorar tu salud ocular.</p>
            </div>
            <div class="mx-auto mt-16 grid max-w-2xl grid-cols-1 gap-x-8 gap-y-20 lg:mx-0 lg:max-w-none lg:grid-cols-3">
                <article v-for="post in posts" :key="post.id" class="flex flex-col items-start justify-between">
                <div class="relative w-full">
                    <img :src="post.imageUrl" alt="" class="aspect-[16/9] w-full rounded-2xl bg-gray-100 object-cover sm:aspect-[2/1] lg:aspect-[3/2]" />
                    <div class="absolute inset-0 rounded-2xl ring-1 ring-inset ring-gray-900/10" />
                </div>
                    <div class="max-w-xl">
                        <div class="group relative">
                        <h3 class="mt-3 text-lg font-semibold leading-6 text-gray-900 group-hover:text-gray-600">
                            <a :href="post.href">
                            <span class="absolute inset-0" />
                            {{ post.title }}
                            </a>
                        </h3>
                            <p class="mt-5 line-clamp-5 text-sm leading-6 text-gray-600">{{ post.description }}</p>
                        </div>
                    </div>
                </article>
            </div>
        </div>
    </div>
</template>

<script setup>
const posts = [
  {
    id: 1,
    title: 'OCULOPLASTICA',
    href: 'https://www.youtube.com/watch?v=9ca5IY9WkTQ',
    description:
      'Nos enfocamos en el diagnóstico y tratamiento de las enfermedades y trastornos que afectan las estructuras alrededor del ojo. Esto incluye los párpados, la órbita (la cavidad donde se aloja el ojo), el sistema lagrimal y las cejas.',
    imageUrl:
      'https://i.postimg.cc/KcNFBz7D/oculoplastica.jpg',
  },
  {
    id: 2,
    title: 'OFTALMOLOGIA PEDIATRICA',
    href: 'https://www.youtube.com/watch?v=GpVBxfIU9Kg',
    description:
      'Nos centramos en el diagnóstico y tratamiento de enfermedades oculares y problemas de visión en niños, desde recién nacidos hasta adolescentes.',
    imageUrl:
      'https://i.postimg.cc/t4NptNxJ/pediatrica.jpg',
  },
  {
    id: 3,
    title: 'RETINA',
    href: 'https://www.youtube.com/watch?v=g2OOm9d6NWk',
    description:
      'Nos dedicamos al diagnóstico y tratamiento de enfermedades y trastornos que afectan la retina, una capa delgada de tejido sensible a la luz en la parte posterior del ojo que es esencial para la visión.',
    imageUrl:
      'https://i.postimg.cc/jjKxfk3L/oftalmologia.jpg',
  },
  {
    id: 4,
    title: 'GLAUCOMA',
    href: 'https://www.youtube.com/watch?v=CjgNi8DjKS8',
    description:
      'Nos centramos en el diagnóstico, tratamiento y manejo de una enfermedad que daña el nervio óptico y puede llevar a la pérdida de la visión, generalmente debido a una presión intraocular elevada',
    imageUrl:
      'https://i.postimg.cc/RZFtJdh1/glaucoma.jpg',
  },
  {
    id: 5,
    title: 'ESTRABISMO',
    href: 'https://www.youtube.com/watch?v=5alPtzcBWLg',
    description:
      'Nos enfocamos en el diagnóstico y tratamiento de la desalineación ocular, es decir, cuando los ojos no están alineados correctamente y miran en diferentes direcciones.',
    imageUrl:
      'https://i.postimg.cc/9QYWVHCJ/estrabismo.jpg',
  },
  {
    id: 6,
    title: 'CORNEA',
    href: 'https://www.youtube.com/watch?v=N6Jvo3zL5YE',
    description:
      'Nos centramos en el diagnóstico, tratamiento y manejo de enfermedades y trastornos que afectan la córnea, que es la capa transparente en la parte frontal del ojo que cubre el iris, la pupila y la cámara anterior.',
    imageUrl:
      'https://i.postimg.cc/rw1pmtCG/cornea.jpg',
  }
]
</script>