<script>
    function fillFromList(id, tags) {
        const template = document.querySelector(`#${id} temp`).innerHTML;

        document.querySelector(`#${id}`).innerHTML = tags.split(', ').map(t => template.replace('##', t)).join(' ');
    }
    
    function repeatTemplate(id, groups) {
        const template = document.querySelector(`#${id} temp`).innerHTML;
        
        document.querySelector(`#${id}`).innerHTML = groups.map(g => {
            let html = template.substr(0);
            g.forEach(t => html = html.replace('##', t));
            return html;
        }).join(' ');
    }

    setTimeout(() => {
        fillFromList('key-tech-exp-list', 'Javascript, C#, Angular, React Native, MongoDB, NodeJS, ASP.NET WebApi2, WPF, Ionic, Microsoft SQL');

        fillFromList('additional-tech-exp-list', 'UX, Svelte, Typescript, Linux, WebTorrent, WebRTC, Python, Unity game engine, web security, compiler design, GraphQL, chat bots, Coffeescript, augmented reality, evolutionary algorithms');

        fillFromList('microbuild-tech-exp-list', 'Angular, ASP.NET WebApi2, MongoDB, Azure, Ionic, Stencil, WebRTC, Android, iOS, WPF');

        fillFromList('x99xt-tech-exp-list', 'AngularJS, NodeJS, ASP.NET WebApi2, MS SQL, SOAP, Xamarin');

        fillFromList('epixcell-tech-exp-list', 'JavaScript, NodeJS, MongoDB, MySQL');

        fillFromList('anantara-tech-list', 'Unity3d, Vuforia, .NET Mono, NodeJS, MongoDB, Android, iOS, React Native, Viro AR');

        fillFromList('donatelk-tech-list', 'React Native, Flow, MongoDB, NodeJS, Microsoft Cognitive Services, Google Maps, Android, iOS');

        fillFromList('ongoinglk-tech-list', 'Angular, Angular Material, NodeJS, MongoDB, NativeScript, HapiJS');

        repeatTemplate('career-status-list', [
            ['Role', 'Senior software engineer'],
            ['Degree', 'BSc. (computer engineering)']
        ]);

        repeatTemplate('web-links-list', [
            ['E-mail', 'nir@nirlanka.com', 'mailto:nir@nirlanka.com'],
            ['LinkedIn', 'linkedin.com/in/nirlanka', 'https://linkedin.com/in/nirlanka'],
            ['GitHub', 'github.com/nirlanka', 'https://github.com/nirlanka'],
            ['Blog', 'evildino.com', 'https://evildino.com'],
            ['Stack Overflow', 'stackoverflow.com/users/1056055/nirmall', 'https://stackoverflow.com/users/1056055/nirmall'],
        ].map(a => [a[0], a[2], a[1]]));
    }, 0);

    document.title = 'Nirmal Lankathilaka';

</script>
        
<header class="[ section top-1 ]">
    <h1 class="[ title h1 bold ][ inline-block right-1 vertical-middle ]">Nirmal Lankathilaka</h1>
    <div class="[ tag-wrapper ][ top-2 vertical-middle ]" style="width: 190px;"><span class="tag medium" style="width: 190px;">Senior software engineer</span></div>
</header>

<section class="section light top-1">
    <a href="https://linkedin.com/in/nirlanka" class="[ gray a ][ right-1 ]">linkedin.com/in/nirlanka</a>
    <a href="mailto:nir@nirlanka.com" class="[ gray a ]">nir@nirlanka.com</a>
</section>

<section class="[ normal ][ section top-1 ]">
    <p class="thin desc">A computer engineering graduate from the University of Peradeniya with 5 years of experience in full-stack development & design for mobile, web, desktop applications & APIs.</p>
</section>

<section class="[ section timeline ][ top-2 row10 ]">
    <div class="col10-1 timeline-item">
        <div class="timeline-graphic">
            <span class="timeline-circle">&nbsp;</span>
            <span class="timeline-line">&nbsp;</span>
        </div>
        <div class="gray thin bottom-1">Today ← Sep. 2019</div>
        <div class="title bottom-2">
            <div class="bold dark-purple">Senior software engineer</div>
            <div class="thin dark-purple">@ <a class="a thin dark-purple" href="http://www.embla.asia/">Embla</a> <a class="a thin dark-purple" href="http://www.microbuild.no/">/MicroBuild</a></div>
        </div>
    </div>
    <div class="col10-2 timeline-item">
        <div class="timeline-graphic">
            <span class="timeline-dot">&nbsp;</span>
            <span class="timeline-line">&nbsp;</span>
        </div>
        <div class="gray thin bottom-1">← Jan. 2017</div>
        <div class="title bottom-2">
            <div class="bold dark-purple">Software engineer</div>
            <div class="thin dark-purple">@ <a class="a thin dark-purple" href="http://www.embla.asia/">Embla</a> <a class="a thin dark-purple" href="http://www.microbuild.no/">/MicroBuild</a></div>
        </div>
    </div>
    <div class="col10-2 timeline-item">
        <div class="timeline-graphic">
            <span class="timeline-dot">&nbsp;</span>
            <span class="timeline-line">&nbsp;</span>
        </div>
        <div class="gray thin bottom-1">Apr. 2016 ← Oct. 2015</div>
        <div class="title bottom-2">
            <div class="bold dark-purple">Associate software engineer</div>
            <div class="thin dark-purple">@ <a class="a thin dark-purple" href="https://www.99xtechnology.com/">99x technology</a> <a class="a thin dark-purple" href="https://www.boligmappa.no/">/Boligmappa</a></div>
        </div>
    </div>
    <div class="col10-2 timeline-item">
        <div class="timeline-graphic">
            <span class="timeline-dot">&nbsp;</span>
            <span class="timeline-line">&nbsp;</span>
        </div>
        <div class="gray thin bottom-1">Apr. 2016 ← Oct. 2015</div>
        <div class="title bottom-2">
            <div class="bold dark-purple">BSc. (Computer engineering) 
</div>
            <div class="thin dark-purple">@ <a class="a thin dark-purple" href="https://eng.pdn.ac.lk/">University of Peradeniya</a> /<a class="a thin dark-purple" href="http://www.ce.pdn.ac.lk/">Engineering Faculty</a></div>
        </div>
    </div>
    <div class="col10-2 timeline-item">
        <div class="timeline-graphic">
            <span class="timeline-dot">&nbsp;</span>
            <span class="timeline-line">&nbsp;</span>
        </div>
        <div class="gray thin bottom-1">Mar. 2013 ← Sep. 2011</div>
        <div class="title bottom-2">
            <div class="bold dark-purple">Trainee software engineer</div>
            <div class="thin dark-purple">@ <span class="thin dark-purple" href="https://www.99xtechnology.com/">ePixcell Pvt Ltd</span></div>
        </div>
    </div>
    <div class="col10-1 timeline-item">
        <div class="timeline-graphic">
            <span class="timeline-dot">&nbsp;</span>
            <span class="timeline-line">&nbsp;</span>
        </div>
        <div class="gray thin bottom-1">Aug. 2011 ← Jan. 2009</div>
        <div class="title bottom-2">
            <div class="bold dark-purple">Advanced Levels in mathematics, physics, chemistry</div>
            <div class="thin dark-purple">(Sri Lanka)</div>
        </div>
    </div>
</section>

<section class="[ section key-tech-exp top-2 ][ row10 ]">
    <div class="col10-2"><h2 class="title medium dark font-2 bottom-1">Key technology experience</h2></div>
    <div class="col10-8 tag-list" id="key-tech-exp-list">
        <temp>
            <div class="tag inline-block">
                ##<span class="invisible">,</span>
            </div>
        </temp>
    </div>
</section>

<section class="[ section additional-tech-exp top-1 ][ row10 ]">
    <div class="col10-2"><h2 class="title medium dark font-2 bottom-1">Additional experience</h2></div>
    <div class="col10-8 tag-list" id="additional-tech-exp-list">
        <temp>
            <div class="[ tag tag-lighter ][ inline-block ]">
                ##<span class="invisible">,</span>
            </div>
        </temp>
    </div>
</section>

<div class="top-2 row10">
    
    <section class="[ section ][ col10-7 bottom-1 ]">
        
        <div class="row10">
            <div class="col-2"><h2 class="title medium dark font-2 bottom-1">Current project</h2></div>
        </div>
        
        <div class="row10 nested">
            <div class="col10-2">
                <div class="dark-blue title top-1">2017 &mdash; Today</div>
            </div>
            <div class="col10-8">
                <h3 class="h3 title dark-blue">
                    <div class="black">Senior software engineer (SE, SSE)</div>
                    <div>at Embla Software Innovation / MicroBuild (Dørteknikk AS)</div>
                </h3>
                
                <div id="microbuild-tech-exp-list" class="tag-list top-1 bottom-1">
                    <temp>
                        <div class="[ tag ][ inline-block ]">
                            ##<span class="invisible">,</span>
                        </div>
                    </temp>
                </div>
                
                <p class="p">I work for Dørteknikk AS (Norway) to design, develop and maintain a software suite of web, mobile and desktop applications.</p>

                <p class="p">There I work with multiple technologies and is responsible for both web, mobile, desktop and back-end development. I am responsible for requirement gathering and communication with the project owner.</p>
                <p class="p">
                    <span class="bold">Website:</span>
                    <a href="http://www.microbuild.no" class="a">microbuild.no</a>
                </p>
                
            </div>
        </div>

        <div class="row10 nested">
            <div class="col10-2">
                <div class="dark-blue title top-1">2015 &mdash; 2016</div>
            </div>
            <div class="col10-8">
                <h3 class="h3 title dark-blue">
                    <div class="black">Associate software engineer</div>
                    <div>at 99x Technology / Boligmappa (AS)</div>
                </h3>
                
                <div id="x99xt-tech-exp-list" class="tag-list top-1 bottom-1">
                    <temp>
                        <div class="[ tag ][ inline-block ]">
                            ##<span class="invisible">,</span>
                        </div>
                    </temp>
                </div>
                
                <p class="p">I worked on Boligmappa AS, a suite of web and mobile apps for tracking, management and document-gathering of electrical appliances for Norwegian homes and buildings.</p>

                <p class="p">My responsibilities also included direct communication with clients and the design and development of solutions.</p>
                <p class="p">
                    <span class="bold">Website:</span>
                    <a href="https://www.boligmappa.no/" class="a">boligmappa.no</a>
                </p>
                
            </div>
        </div>

        <div class="row10 nested">
            <div class="col10-2">
                <div class="dark-blue title top-1">2011 &mdash; 2013</div>
            </div>
            <div class="col10-8">
                <h3 class="h3 title dark-blue">
                    <div class="black">Trainee software engineer</div>
                    <div>at ePixcell Pvt Ltd</div>
                </h3>
                
                <div id="epixcell-tech-exp-list" class="tag-list top-1 bottom-1">
                    <temp>
                        <div class="[ tag ][ inline-block ]">
                            ##<span class="invisible">,</span>
                        </div>
                    </temp>
                </div>
                
                <p class="p">I started as a web designer and developer and moved mainly to web application development.</p>

                <p class="p">We worked with a number of foreign and local clients on web apps and integrations that helped in financial and enterprise solutions.</p>
                
            </div>
        </div>
        
        <div class="row10 top-2">
            <div class="col-2"><h2 class="title medium dark font-2 bottom-1">Other projects</h2></div>
        </div>
        
        <div class="row10 nested">
            <div class="col10-2">
                <div class="col10-2">
                    <div class="dark-blue title top-1">2019</div>
                </div>
            </div>
            <div class="col10-8">
                <h2 class="dark-purple title h3"><span class="bold">Anantara AR Experience</span> (for Triolly Pvt. Ltd.)</h2>
                <div id="anantara-tech-list" class="tag-list top-1 bottom-1">
                    <temp>
                        <div class="[ tag ][ inline-block ]">
                            ##<span class="invisible">,</span>
                        </div>
                    </temp>
                </div>
                
                <p class="p">An augmented-reality virtual tour app for Anantara Kalutara Resort by Anantara Hotels, Resorts & Spas, a successful hotel chain covering a dozen countries.</p>
                <p class="p">I developed this using the Unity engine, Vuforia augmented reality and .NET. We used BLE Bluetooth beacons for automating the virtual tour experience based on location. I developed the proof-of-concept in React Native and Viro AR.
                </p>
                <div class="p">
                    <div>
                        <span class="bold">Apple:</span>
                        <a href="https://apps.apple.com/lk/app/anantara-ar-experience/id1474047633" class="a">Anantara AR Experience on App Store</a>
                    </div>
                    <div>
                        <span class="bold">Android:</span>
                        <a href="https://play.google.com/store/apps/details?id=com.triolly.anantaraexp&hl=en_CA" class="a">Anantara AR Experience on Play Store</a>
                    </div>
                </div>
                
            </div>
        </div>

        <div class="row10 nested">
            <div class="col10-2">
                <div class="col10-2">
                    <div class="dark-blue title top-1">2017</div>
                </div>
            </div>
            <div class="col10-8">
                <h2 class="dark-purple title h3"><span class="bold">Donate LK</span></h2>
                <div id="donatelk-tech-list" class="tag-list top-1 bottom-1">
                    <temp>
                        <div class="[ tag ][ inline-block ]">
                            ##<span class="invisible">,</span>
                        </div>
                    </temp>
                </div>
                
                <p class="p">An augmented-reality virtual tour app for Anantara Kalutara Resort by Anantara Hotels, Resorts & Spas, a successful hotel chain covering a dozen countries.</p>
                <p class="p">I developed this using the Unity engine, Vuforia augmented reality and .NET. We used BLE Bluetooth beacons for automating the virtual tour experience based on location. I developed the proof-of-concept in React Native and Viro AR.</p>
                
            </div>
        </div>

        <div class="row10 nested">
            <div class="col10-2">
                <div class="col10-2">
                    <div class="dark-blue title top-1">2017</div>
                </div>
            </div>
            <div class="col10-8">
                <h2 class="dark-purple title h3"><span class="bold">Ongoing LK</span></h2>
                <div id="ongoinglk-tech-list" class="tag-list top-1 bottom-1">
                    <temp>
                        <div class="[ tag ][ inline-block ]">
                            ##<span class="invisible">,</span>
                        </div>
                    </temp>
                </div>
                
                <p class="p">Responsive web app and mobile app for keeping up with tickets, offers, and discounts on movies, shows, clothes, dining.</p>
                <p class="p">I used Angular and Angular Universal for developing and fast-delivering the web application, and NativeScript with Angular for the cross-platform app. We developed the back-end with NodeJS, HapiJS and MongoDB.</p>
                <p class="p">We adhered to material design guidelines as well as responsive design principals to design a seamless experience between both mobile app and web app.</p>
                
            </div>
        </div>
        
    </section>
    
    <section class="[ section sidebar ][ col10-3 ]">
        <h3 class="title medium font-2 top-1 bottom-1">Career status</h3>
        
        <div id="career-status-list">
            <temp>
                <div class="p">
                    <div class="inline-block min-w-100 title dark-purple bold">##</div>
                    <div class="inline-block min-w-200 break-words">##</div>
                </div>
            </temp>
        </div>
        
        <h3 class="title medium font-2 top-1 bottom-1">Links</h3>
        
        <div id="web-links-list">
            <temp>
                <div class="p">
                    <div class="inline-block min-w-100 max-w-100 title dark-purple bold">##</div>
                    <div class="inline-block min-w-200 max-w-200 break-words">
                        <a href="##" class="a inline">##</a>
                    </div>
                </div>
            </temp>
        </div>
        
    </section>
    
</div>

<div class="bottom-2">&nbsp;</div>