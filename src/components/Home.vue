<template>
	<nav class="navbar navbar-expand-lg navbar-light bg-white border-bottom sticky-top py-3">
		<div class="container">
			<a class="navbar-brand d-flex align-items-center fw-bold text-dark fs-4" href="#">
				<span class="d-inline-flex align-items-center justify-content-center bg-primary text-white rounded me-2 px-2 py-1 fs-6">
					&lt;/&gt;
				</span>
				BytePath
			</a>
			<button 
			class="navbar-toggler border-0 shadow-none" 
			type="button" 
			data-bs-toggle="collapse" 
			data-bs-target="#navbarNav" 
			aria-controls="navbarNav" 
			aria-expanded="false" 
			aria-label="Toggle navigation"
			>
			<span class="navbar-toggler-icon"></span>
			</button>

			<div class="collapse navbar-collapse" id="navbarNav">
				<ul class="navbar-nav ms-auto align-items-lg-center gap-lg-1">
					<li class="nav-item"><a class="nav-link active fw-medium text-primary px-3" aria-current="page" href="#home">Home</a></li>
					<li class="nav-item"><a class="nav-link fw-medium text-secondary px-3" href="#introduction">Introduction</a></li>
					<li class="nav-item"><a class="nav-link fw-medium text-secondary px-3" href="#featured">Featured</a></li>
					<li class="nav-item"><a class="nav-link fw-medium text-secondary px-3" href="#categories-section">Categories</a></li>
					<li class="nav-item"><a class="nav-link fw-medium text-secondary px-3" href="#resources">Resources</a></li>
					<li class="nav-item"><a class="nav-link fw-medium text-secondary px-3" href="#about">About</a></li>
					<li class="nav-item ms-lg-3 mt-2 mt-lg-0">
						<a href="#about" class="btn btn-outline-secondary btn-sm px-3 me-2 fw-medium">Sign In</a>
						<a href="#featured" class="btn btn-primary btn-sm px-3 fw-medium">Get Started</a>
					</li>
				</ul>
			</div>
		</div>
	</nav>

	<section id="home" class="py-5 bg-white border-bottom">
		<div class="container py-lg-5">
			<div class="row align-items-center g-5">
				<div class="col-lg-6">
					<div class="d-inline-flex align-items-center gap-2 px-3 py-1 mb-3 rounded-pill bg-light border text-muted small fw-medium">
						<span class="rounded-circle bg-success d-inline-block" style="width: 10px; height: 10px;"></span>
						<span>Open Beta • Interactive Learning Tracks</span>
					</div>
					<h1 class="display-4 fw-bold text-dark lh-sm mb-3">
						Master Modern Code, from <span class="text-primary">First Byte</span> to Production.
					</h1>
					<p class="lead text-secondary mb-4">
						Curated roadmaps, hands-on interactive modules, and comprehensive resources engineered for self-taught software engineers and CS students.
					</p>
					<div class="d-flex flex-wrap gap-3 mb-5">
						<a href="#featured" class="btn btn-primary btn-lg px-4 shadow-sm fw-medium">
							Get Started Free <i class="bi bi-arrow-right ms-1"></i>
						</a>
						<a href="#categories-section" class="btn btn-outline-secondary btn-lg px-4 fw-medium">
							Explore Catalog
						</a>
					</div>

					<div class="row g-4 pt-3 border-top">
						<div class="col-4">
							<div class="h3 fw-bold text-dark mb-0">38+</div>
							<div class="small text-muted">Production Paths</div>
						</div>
						<div class="col-4">
							<div class="h3 fw-bold text-dark mb-0">14.2k</div>
							<div class="small text-muted">Active Learners</div>
						</div>
						<div class="col-4">
							<div class="h3 fw-bold text-dark mb-0">99.4%</div>
							<div class="small text-muted">Pass Rate</div>
						</div>
					</div>
				</div>

				<div class="col-lg-6">
					<div class="card border rounded-4 shadow-sm overflow-hidden bg-light">
						<div class="card-header bg-white border-bottom py-2 px-3 d-flex align-items-center justify-content-between">
							<div class="d-flex align-items-center gap-2">
								<span class="rounded-circle bg-danger d-inline-block" style="width: 10px; height: 10px;"></span>
								<span class="rounded-circle bg-warning d-inline-block" style="width: 10px; height: 10px;"></span>
								<span class="rounded-circle bg-success d-inline-block" style="width: 10px; height: 10px;"></span>
								<span class="small font-monospace text-muted ms-2">sandbox.bytepath.dev</span>
							</div>
							<span class="badge bg-success-subtle text-success border border-success-subtle font-monospace">ACTIVE RUNTIME</span>
						</div>
						<div class="card-body p-4 bg-light font-monospace small lh-base text-dark">
							<div class="text-muted mb-2"># LRU Cache implementation with O(1) eviction</div>
							<div><span class="text-primary fw-bold">class</span> <span class="text-dark fw-bold">LRUCache</span>:</div>
							<div class="ps-3"><span class="text-primary fw-bold">def</span> <span class="text-info-emphasis">__init__</span>(self, capacity: <span class="text-success">int</span>):</div>
							<div class="ps-5 text-secondary">self.cap = capacity</div>
							<div class="ps-5 text-secondary">self.cache = OrderedDict()</div>
							<div class="ps-3 mt-2"><span class="text-primary fw-bold">def</span> <span class="text-info-emphasis">get</span>(self, key: <span class="text-success">int</span>) -&gt; <span class="text-success">int</span>:</div>
							<div class="ps-5 text-secondary"><span class="text-primary fw-bold">if</span> key <span class="text-primary fw-bold">not in</span> self.cache: <span class="text-primary fw-bold">return</span> -1</div>
							<div class="ps-5 text-secondary">self.cache.move_to_end(key)</div>
							<div class="ps-5 text-secondary"><span class="text-primary fw-bold">return</span> self.cache[key]</div>
						</div>
						<div class="card-footer bg-white border-top py-2 px-3 d-flex justify-content-between align-items-center small text-muted font-monospace">
							<span><i class="text-success me-1">✓</i> Typecheck Clean (0 errors)</span>
							<span>Latency: 14ms</span>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>

	<section id="introduction" class="py-5 bg-light border-bottom">
		<div class="container py-lg-4">
			<div class="text-center mx-auto mb-5" style="max-width: 680px;">
				<span class="text-uppercase text-primary font-monospace small fw-bold">Architectural Methodology</span>
				<h2 class="display-6 fw-bold text-dark mt-2 mb-3">Engineering education designed for deep technical intuition.</h2>
				<p class="text-secondary">BytePath strips away superficial tutorial purgatory and replaces it with structured cognitive scaffolding and real-world system patterns.</p>
			</div>

			<div class="row g-4">
				<div class="col-md-4">
					<div class="card h-100 border rounded-3 p-4 bg-white shadow-sm">
						<div class="rounded-3 bg-primary-subtle text-primary d-inline-flex align-items-center justify-content-center p-3 mb-3" style="width: 48px; height: 48px;">
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2v20M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>
						</div>
						<h5 class="fw-bold text-dark mb-2">Structured Roadmaps</h5>
						<p class="text-secondary small mb-3">Step-by-step verified learning paths sequenced from prerequisite concepts to production microservices.</p>
						<a href="#featured" class="text-primary small fw-semibold text-decoration-none mt-auto">Dependency graph verification &rarr;</a>
					</div>
				</div>
				<div class="col-md-4">
					<div class="card h-100 border rounded-3 p-4 bg-white shadow-sm">
						<div class="rounded-3 bg-primary-subtle text-primary d-inline-flex align-items-center justify-content-center p-3 mb-3" style="width: 48px; height: 48px;">
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
						</div>
						<h5 class="fw-bold text-dark mb-2">Hands-on Challenges</h5>
						<p class="text-secondary small mb-3">In-browser code exercises, instant feedback test runners, and real architectural mini-projects.</p>
						<a href="#featured" class="text-primary small fw-semibold text-decoration-none mt-auto">Automated test suites &rarr;</a>
					</div>
				</div>
				<div class="col-md-4">
					<div class="card h-100 border rounded-3 p-4 bg-white shadow-sm">
						<div class="rounded-3 bg-primary-subtle text-primary d-inline-flex align-items-center justify-content-center p-3 mb-3" style="width: 48px; height: 48px;">
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z"/></svg>
						</div>
						<h5 class="fw-bold text-dark mb-2">Curated Tooling</h5>
						<p class="text-secondary small mb-3">Vetted open-source libraries, deep-dive specification docs, and production cheat sheets curated by senior engineers.</p>
						<a href="#resources" class="text-primary small fw-semibold text-decoration-none mt-auto">Production ready benchmarks &rarr;</a>
					</div>
				</div>
			</div>
		</div>
	</section>

	<section id="featured" class="py-5 bg-white border-bottom">
		<div class="container py-lg-4">
			<div class="d-flex flex-column flex-md-row justify-content-between align-items-md-end mb-4 gap-3">
				<div>
					<span class="text-uppercase text-primary font-monospace small fw-bold">Recommended Curriculum</span>
					<h2 class="display-6 fw-bold text-dark mb-1">Featured Tracks</h2>
					<p class="text-secondary mb-0">Accelerated industry blueprints built for direct engineering mastery.</p>
				</div>
				<div class="btn-group" role="group">
					<button type="button" class="btn btn-sm btn-primary active">All Tracks</button>
					<button type="button" class="btn btn-sm btn-outline-secondary">Frontend</button>
					<button type="button" class="btn btn-sm btn-outline-secondary">Backend</button>
					<button type="button" class="btn btn-sm btn-outline-secondary">Systems &amp; Algo</button>
				</div>
			</div>

			<div class="row g-4">
				<div class="col-lg-4 col-md-6">
					<div class="card h-100 border rounded-4 overflow-hidden shadow-sm">
						<div class="p-4 bg-light border-bottom text-center position-relative">
							<div class="d-flex justify-content-between position-absolute top-0 start-0 w-100 p-3">
								<span class="badge bg-white text-primary border shadow-sm">BEGINNER</span>
								<span class="small fw-semibold text-warning">★ 4.90</span>
							</div>
							<div class="py-4 mt-2">
								<svg width="60" height="60" viewBox="0 0 64 64" fill="none" stroke="#4f46e5" stroke-width="2">
									<rect x="12" y="16" width="40" height="8" rx="2"/>
									<rect x="16" y="28" width="32" height="8" rx="2"/>
									<rect x="20" y="40" width="24" height="8" rx="2"/>
								</svg>
							</div>
						</div>
						<div class="card-body p-4 d-flex flex-column">
							<div class="d-flex gap-1 mb-2 font-monospace small text-muted">
								<span>HTML5</span> • <span>Modern CSS</span> • <span>Vue.js</span> • <span>Node.js</span>
							</div>
							<h5 class="card-title fw-bold text-dark mb-2">Full-Stack Web Foundations</h5>
							<p class="card-text text-secondary small flex-grow-1">Construct modern, accessible single-page client applications backed by REST APIs, reactive state, and modern CSS architecture.</p>
							<div class="d-flex justify-content-between align-items-center pt-3 border-top mt-3 small">
								<span class="text-muted"><i class="bi bi-clock me-1"></i>40 hrs</span>
								<a href="#" class="btn btn-outline-primary btn-sm fw-medium">Start Track &rarr;</a>
							</div>
						</div>
					</div>
				</div>

				<div class="col-lg-4 col-md-6">
					<div class="card h-100 border rounded-4 overflow-hidden shadow-sm">
						<div class="p-4 bg-light border-bottom text-center position-relative">
							<div class="d-flex justify-content-between position-absolute top-0 start-0 w-100 p-3">
								<span class="badge bg-white text-info-emphasis border shadow-sm">INTERMEDIATE</span>
								<span class="small fw-semibold text-warning">★ 4.95</span>
							</div>
							<div class="py-4 mt-2">
								<svg width="60" height="60" viewBox="0 0 64 64" fill="none" stroke="#0ea5e9" stroke-width="2">
									<circle cx="32" cy="18" r="8"/><circle cx="20" cy="44" r="8"/><circle cx="44" cy="44" r="8"/>
									<line x1="28" y1="24" x2="23" y2="38"/><line x1="36" y1="24" x2="41" y2="38"/><line x1="28" y1="44" x2="36" y2="44"/>
								</svg>
							</div>
						</div>
						<div class="card-body p-4 d-flex flex-column">
							<div class="d-flex gap-1 mb-2 font-monospace small text-muted">
								<span>Go</span> • <span>PostgreSQL</span> • <span>Docker</span> • <span>gRPC</span>
							</div>
							<h5 class="card-title fw-bold text-dark mb-2">Modern Backend &amp; Distributed Systems</h5>
							<p class="card-text text-secondary small flex-grow-1">Engineer fault-tolerant backend architectures, relational data stores, high-concurrency microservices, and container pipelines.</p>
							<div class="d-flex justify-content-between align-items-center pt-3 border-top mt-3 small">
								<span class="text-muted"><i class="bi bi-clock me-1"></i>60 hrs</span>
								<a href="#" class="btn btn-outline-primary btn-sm fw-medium">Start Track &rarr;</a>
							</div>
						</div>
					</div>
				</div>

				<div class="col-lg-4 col-md-6">
					<div class="card h-100 border rounded-4 overflow-hidden shadow-sm">
						<div class="p-4 bg-light border-bottom text-center position-relative">
							<div class="d-flex justify-content-between position-absolute top-0 start-0 w-100 p-3">
								<span class="badge bg-white text-secondary border shadow-sm">ALL LEVELS</span>
								<span class="small fw-semibold text-warning">★ 4.88</span>
							</div>
							<div class="py-4 mt-2">
								<svg width="60" height="60" viewBox="0 0 64 64" fill="none" stroke="#6366f1" stroke-width="2">
									<circle cx="32" cy="16" r="6"/><circle cx="20" cy="32" r="6"/><circle cx="44" cy="32" r="6"/>
									<circle cx="14" cy="48" r="5"/><circle cx="26" cy="48" r="5"/>
									<line x1="28" y1="21" x2="23" y2="27"/><line x1="36" y1="21" x2="41" y2="27"/>
								</svg>
							</div>
						</div>
						<div class="card-body p-4 d-flex flex-column">
							<div class="d-flex gap-1 mb-2 font-monospace small text-muted">
								<span>Python</span> • <span>LeetCode 150</span> • <span>Big-O</span>
							</div>
							<h5 class="card-title fw-bold text-dark mb-2">Applied Data Structures &amp; Algorithms</h5>
							<p class="card-text text-secondary small flex-grow-1">Internalize core computational models, recursive patterns, graph traversal heuristics, and memory trade-offs for technical interviews.</p>
							<div class="d-flex justify-content-between align-items-center pt-3 border-top mt-3 small">
								<span class="text-muted"><i class="bi bi-clock me-1"></i>35 hrs</span>
								<a href="#" class="btn btn-outline-primary btn-sm fw-medium">Start Track &rarr;</a>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>