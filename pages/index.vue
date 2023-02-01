<template>
    <div class="h-max-screen w-max-screen leading-relaxed antialiased">
        <!-- nav -->
        <div
            class="flex items-center justify-between h-90 bg-blue-800 px-6 py-2 md:px-20 md:py-4"
        >
            <div class="w-10 h-10 md:w-20 md:h-20">
                <img
                    src="~/assets/images/logo.png"
                    alt="ARW Homestay - Homestay nyaman di bantul, yogyakarta"
                />
            </div>
            <div class="hidden md:block">
                <ul class="flex space-x-8 w-full items-center h-full">
                    <li class="text-white uppercase text-base">
                        <a href="#">Home</a>
                    </li>
                    <li class="text-white uppercase text-base">
                        <a href="#information">Informasi</a>
                    </li>
                    <li class="text-white uppercase text-base">
                        <a href="#">Penawaran</a>
                    </li>
                    <li class="text-white uppercase text-base">
                        <a href="#">Paket</a>
                    </li>
                    <li class="text-white uppercase text-base">
                        <a href="#">Fasilitas</a>
                    </li>
                    <li class="text-white uppercase text-base">
                        <a href="#">Galeri Foto</a>
                    </li>
                    <li
                        class="text-white uppercase text-base px-3 py-2 bg-white text-blue-800"
                    >
                        <a href="#">Pesan Sekarang</a>
                    </li>
                </ul>
            </div>
            <div class="md:hidden" @click="nav = !nav">
                <svg
                    v-if="!nav"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-8 h-8 text-white"
                >
                    <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
                    />
                </svg>

                <svg
                    v-if="nav"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="w-8 h-8 text-white"
                >
                    <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        d="M6 18L18 6M6 6l12 12"
                    />
                </svg>
            </div>
        </div>
        <!-- mobile nav -->
        <div class="md:hidden bg-blue-800" v-if="nav">
            <ul class="w-full">
                <li
                    class="px-4 py-2 text-white hover:bg-blue-700"
                    @click="nav = !nav"
                >
                    <a href="#">Home</a>
                </li>
                <li
                    class="px-4 py-2 text-white hover:bg-blue-700"
                    @click="nav = !nav"
                >
                    <a href="#information">Informasi</a>
                </li>
                <li
                    class="px-4 py-2 text-white hover:bg-blue-700"
                    @click="nav = !nav"
                >
                    <a href="#">Penawaran</a>
                </li>
                <li
                    class="px-4 py-2 text-white hover:bg-blue-700"
                    @click="nav = !nav"
                >
                    <a href="#">Paket</a>
                </li>
                <li
                    class="px-4 py-2 text-white hover:bg-blue-700"
                    @click="nav = !nav"
                >
                    <a href="#">Fasilitas</a>
                </li>
                <li class="px-6 py-4 text-right">
                    <a href="#" class="bg-white text-blue-800 px-4 py-2"
                        >Pesan Sekarang</a
                    >
                </li>
            </ul>
        </div>

        <!-- carousel -->
        <carousel :autoplay="true" :paginationPadding="5" :perPage="1">
            <slide>
                <div class="relative">
                    <img class="w-full" src="~/assets/images/foto1.svg" />
                    <div
                        class="absolute hidden md:block right-20 w-80 bottom-24 text-justify bg-blue-800 text-white p-2 font-bold"
                    >
                        Gerbang luar yang bisa untuk memarkirkan kendaraan Anda.
                    </div>
                </div>
            </slide>
            <slide>
                <div class="relative">
                    <img class="w-full" src="~/assets/images/foto2.svg" />
                    <div
                        class="absolute hidden md:block right-20 w-80 bottom-24 text-justify bg-blue-800 text-white p-2 font-bold"
                    >
                        Tempat tidur nyaman, untuk istirahat selama liburan
                        Anda.
                    </div>
                </div>
            </slide>
            <slide>
                <div class="relative">
                    <img class="w-full" src="~/assets/images/foto3.svg" />
                    <div
                        class="absolute hidden md:block right-20 w-80 bottom-24 text-justify bg-blue-800 text-white p-2 font-bold"
                    >
                        Suasana malam yang hangat dan tenang.
                    </div>
                </div>
            </slide>
        </carousel>

        <!-- information section -->
        <div id="information" class="h-auto px-8 py-4">
            <div class="border border-2 border-blue-800 px-10 py-6">
                <div
                    class="text-center text-blue-800 font-bold text-2xl pb-4 uppercase"
                >
                    Informasi
                </div>
                Homestay ARW terletak di pinggir jalan umum dan di tengah
                persawahaan dengan udara sejuk dan segar membuat hati nyaman
                yang cocok untuk tempat tinggal sesaat untuk megistirahatkan
                pikiran, jiwa, dan raga. Nama ARW berasal dari nama inisial
                anak-anak pemilik homestay tersebut. Homestay ARW menyediakan 3
                kamar minimalis dengan fasilitas lengkap dan kamar mandi dalam.
                Halaman parkir cukup luas bias muat 5 mobil dengan pengaman
                gerbang kokoh. Living room serasa lega karena rumah didesain
                dengan ventilasi yang sempurna banyak kaca yang bisa dibuka
                untuk menghirup udara segar pedesaan dan sliding kaca besar
                sebagai penerang living room. Letak Homestay ARW berada di
                sekitar pusat Sate Klatak yang berada di seputaran jalan imogiri
                dan tongseng Ayam Kampung. Banyak juga tempat wisata alam yang
                dekat dengan Homestay ARW, seperti Hutan Pinus, Puncak Gebang,
                Puncak Sosok, Puncak Becici, Ziarah Makam Imogiri, Kota gede,
                Pantai, dan masih banyak yang lain. Selain itu homestay ARW juga
                dekat dengan pusat perkotaan, hanya sekitar 20 menit sampai
                Malioboro dan 4 menit sampai Terminal Besar Giwangan. Homestay
                ARW juga menyediakan paket wisata dan sarana transportasi jika
                ingin pergi ke setiap sudut kota jogja dan tidak hafal arah
                ataupun tempat yang nyaman. Kami akan merekomendasikan tempat
                wisata yang tepat, tempat kuliner legendaris, dengan sopir yang
                sopan dan ramah. Harga sarana wisata dan tranportasi Homestay
                ARW relatif murah, aman, dan nyaman (armada bisa pilih sesuai
                keinginan).
            </div>
        </div>

        <!-- package -->
        <div class="bg-blue-800 h-min-screen px-8 py-6">
            <div class="container mx-auto">
                <div id="paket" class="mb-8">
                    <div
                        class="w-full text-center text-white font-bold uppercase text-2xl mb-4"
                    >
                        PAKET
                    </div>
                    <div class="lg:flex lg:items-center lg:-mx-2">
                        <div class="mb-4 lg:mb-0 lg:w-1/3 lg:px-2">
                            <div
                                class="text-center bg-white text-blue-900 p-10"
                            >
                                <h2 class="font-bold mb-4 text-2xl">Weekday</h2>
                                <div class="mb-6">
                                    <span
                                        class="block text-2xl pb-2 line-through"
                                        >Rp. 1.200.000</span
                                    >
                                    <span class="block text-5xl pb-2"
                                        >Rp. 1.000.000</span
                                    >
                                    <span class="text-sm text-grey"
                                        >Per day</span
                                    >
                                </div>
                                <a
                                    class="text-sm tracking-wide uppercase inline-block bg-blue-900 text-white border border-red text-red font-bold w-full p-3 no-underline hover:rotate-3"
                                    href="https://wa.me/6287839127936?text=Hallo%2C%20saya%20ingin%20membooking%20homestay%2C%20paket%20family%20room%20weekday"
                                    >Pesan Sekarang</a
                                >
                            </div>
                        </div>
                        <div class="mb-4 lg:mb-0 lg:w-1/3 lg:px-2">
                            <div
                                class="text-center bg-white text-blue-900 p-10 lg:py-16 lg:shadow-lg"
                            >
                                <h2 class="font-bold mb-4 text-2xl">
                                    Weekend/National Holiday
                                </h2>
                                <div class="mb-6">
                                    <span
                                        class="block text-2xl pb-2 line-through"
                                        >Rp. 1.500.000</span
                                    >
                                    <span class="block text-5xl pb-2"
                                        >Rp. 1.250.000</span
                                    >
                                    <span class="text-sm text-grey"
                                        >Per day</span
                                    >
                                </div>
                                <a
                                    class="text-sm tracking-wide uppercase inline-block bg-blue-900 text-white border border-red text-red font-bold w-full p-3 no-underline hover:rotate-3"
                                    href="https://wa.me/6287839127936?text=Hallo%2C%20saya%20ingin%20membooking%20homestay%2C%20paket%20family%20room%weekend"
                                    >Pesan Sekarang</a
                                >
                            </div>
                        </div>
                        <div class="mb-4 lg:mb-0 lg:w-1/3 lg:px-2">
                            <div
                                class="text-center bg-white text-blue-900 p-10"
                            >
                                <h2 class="font-bold mb-4 text-2xl">
                                    Peak Season
                                </h2>
                                <div class="mb-6">
                                    <span
                                        class="block text-2xl pb-2 line-through"
                                        >Rp. 2.000.000</span
                                    >
                                    <span class="block text-5xl pb-2"
                                        >Rp. 1.500.000</span
                                    >
                                    <span class="text-sm text-grey"
                                        >Per day</span
                                    >
                                </div>
                                <a
                                    class="text-sm tracking-wide uppercase inline-block bg-blue-900 text-white border border-red text-red font-bold w-full p-3 no-underline hover:rotate-3"
                                    href="https://wa.me/6287839127936?text=Hallo%2C%20saya%20ingin%20membooking%20homestay%2C%20paket%20family%20room%20libur%20libur%20nasional"
                                    >Pesan Sekarang</a
                                >
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- facility -->
        <div id="fasilitas" class="px-8 py-4">
            <div
                class="w-full text-center text-blue-900 font-bold uppercase text-2xl mb-4"
            >
                FASILITAS
            </div>
            <div class="lg:flex block lg:space-x-4 space-y-4 lg:space-y-0">
                <div class="border w-full p-5">
                    <div class="lg:flex block">
                        <div>
                            <div class="font-semibold uppercase py-2">
                                Fasilitas
                            </div>
                            <div class="capitalize">
                                <li>Parkir Luas</li>
                                <li>Wifi</li>
                                <li>AC</li>
                                <li>3 Kamar Tidur</li>
                                <li>Kamar Mandi Dalam</li>
                                <li>TV di Living Room</li>
                                <li>
                                    Ruang Keluarga Luas Menyatu dengan Ruang
                                    Makan
                                </li>
                                <li>Mini Bar</li>
                                <li>Dapur Kering</li>
                                <li>Penjaga 24 Jam</li>
                                <li>Teras Depan, Belakang, Samping</li>
                                <li>Taman</li>
                                <li>Pinjam Sepeda / Scooter Gratis</li>
                            </div>
                        </div>
                        <div>
                            <div class="font-semibold uppercase py-2">
                                In Charge
                            </div>
                            <div class="capitalize">
                                <li>Laundry</li>
                                <li>Antar jemput Bandara/Stasiun</li>
                                <li>Paket Wisata</li>
                                <li>Extra bed @50.000</li>
                                <li>Extra person @35.000</li>
                                <li>
                                    Weekend, libur nasional, Hari Raya, dan Cuti
                                    bersama akan dikenakan biaya tambahan
                                </li>
                            </div>
                            <div class="font-semibold uppercase py-2">
                                Transportasi
                            </div>
                            <div class="capitalize">
                                <li>25 Menit dari Bandara Adisucipto</li>
                                <li>25 menit dari Stasiun Lempuyangan</li>
                                <li>30 menit dari Stasiun Tugu Yogyakarta</li>
                                <li>
                                    60 menit dari Bandara Yogyakarta
                                    International Airport
                                </li>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="border w-full p-5 block lg:flex">
                    <div>
                        <div class="font-semibold uppercase py-2">
                            Transportasi
                        </div>
                        <li>25 Menit dari Bandara Adisucipto</li>
                        <li>25 menit dari Stasiun Lempuyangan</li>
                        <li>30 menit dari Stasiun Tugu Yogyakarta</li>
                        <li>
                            60 menit dari Bandara Yogyakarta International
                            Airport
                        </li>

                        <div class="font-semibold uppercase py-2">
                            Kuliner Legendaris dan Viral
                        </div>
                        <li>2 menit ke Sate Klatak Pak Bari</li>
                        <li>3 menit ke Sate Klatak Pak Pong</li>
                        <li>
                            4 menit ke Bakso Rusuk dan Bakso Lobster Kang Har
                        </li>
                        <li>5 menit ke Mie Ayam Tumini</li>
                        <li>5 menit ke Soto Tahu Kemasan Mbah Wongso</li>
                        <li>6 menit ke Gudeg Yu Sum</li>
                        <li>10 menit ke Ingkung Kuali parangtritis</li>
                        <li>15 menit ke Mangut Lele Mbah Marto</li>
                        <li>15 menit ke Bakmi Jowo Mbak Gito</li>
                        <li>15 menit ke Bakmi Jawa Mbah Mo</li>
                        <li>15 menit ke Tongseng Ayam Sudimoro</li>
                        <li>17 menit ke pecel belut mbah Warno</li>
                        <li>17 menit ke Ayam Goreng Jawa Mbah Cemplung</li>
                    </div>
                    <div>
                        <div class="font-semibold uppercase py-2">
                            Mall Jogja
                        </div>
                        <li>15 menit ke Ambarukmo Plaza</li>
                        <li>16 menit ke Lippo Plaza</li>
                        <li>18 menit ke Galeria Mall</li>
                        <li>20 menit ke Malioboro Mall</li>
                        <li>20 menit ke Hartono Mall</li>
                        <li>25 menit ke Jogja City Mall</li>
                        <li>30 menit ke Sleman city Hall</li>
                        <div class="font-semibold uppercase py-2">
                            Wisata Jogja
                        </div>
                        <li>15 menit ke Alun-alun Kidul</li>
                        <li>16 menit ke Alun-alun Utara</li>
                        <li>16 menit ke Puncak Sosok</li>
                        <li>16 menit ke Makam Raja Imogiri</li>
                        <li>20 menit ke Hutan Pinus Imogiri</li>
                        <li>21 menit ke Puncak Becici</li>
                        <li>25 menit ke Pantai Parangtritis</li>
                        <li>26 menit ke Pantai Depok</li>
                        <li>30 menit ke Pantai Goa Cemara</li>
                        <li>32 menit ke Pantai Baru</li>
                    </div>
                </div>
            </div>
        </div>

        <!-- gallery -->
        <div class="px-8 py-4">
            <div class="grid grid-cols-4 grid-rows-6 grid-flow-col gap-2">
                <div class="w-full col-span-4">
                    <img
                        src="~/assets/images/meta.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>
                <div class="w-full row-span-2">
                    <img
                        src="~/assets/images/gallery5.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>
                <div class="w-full col-span-2 row-span-2">
                    <img
                        src="~/assets/images/gallery3.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>
                <div class="w-full col-span-2">
                    <img
                        src="~/assets/images/kamar1.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>
                <div class="w-full">
                    <img
                        src="~/assets/images/gallery6.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>
                <div class="w-full">
                    <img
                        src="~/assets/images/gallery2.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>
                <div class="w-full col-span-2 row-span-2">
                    <img
                        src="~/assets/images/gallery1.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>

                <div class="w-full col-span-2">
                    <img
                        src="~/assets/images/gallery7.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>

                <div class="w-full col-span-2">
                    <img
                        src="~/assets/images/gallery4.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>
                <div class="w-full col-span-2">
                    <img
                        src="~/assets/images/kamar2.svg"
                        class="inset-0 h-full w-full object-cover object-center rounded opacity-75 hover:opacity-100"
                    />
                </div>
            </div>
        </div>

        <!-- maps -->
        <iframe
            src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d15809.110391274908!2d110.4017374!3d-7.865992!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x974e8ba67093a543!2sHome%20Stay%20ARW!5e0!3m2!1sid!2sid!4v1638069995911!5m2!1sid!2sid"
            height="300"
            class="w-full border-0"
            allowfullscreen=""
            loading="lazy"
        ></iframe>

        <!-- footer -->
        <div class="w-full bg-blue-900">
            <div class="text-white">
                <div class="md:w-1/2 p-5 md:text-left">
                    <div class="my-6 ml-3">
                        <div class="text-xl font-semibold">HOMESTAY ARW</div>
                        <span
                            >Jl. Kanggotan II, Keputren, Pleret, Kec. Pleret,
                            Kabupaten Bantul, Daerah Istimewa Yogyakarta
                            55791</span
                        >
                    </div>
                    <p class="p-3 text-gray-400">
                        Homestay, nyaman saat anda mencari tempat beristirahat
                        saat berwisata di yogyakarta, bantul, jogja. suasana
                        nyaman dan sejuk cocok untuk berlibur bersama keluarga
                    </p>
                    <div
                        class="p-3 text-white-400 font-semibold md:flex space-x-6"
                    >
                        <a href="https://wa.me/6287839127936">Whatsapp</a>
                        <a href="https://instagram.com/homestay_arw"
                            >Instagram</a
                        >
                        <a href="assets/rules.pdf" target="_blank">Peraturan</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";
export default {
    name: "IndexPage",
    components: {
        Carousel,
        Slide,
    },
    data() {
        return {
            nav: false,
        };
    },
};
</script>
