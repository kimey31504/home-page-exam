<template>
	<section id="about" class="py-5 bg-white border-bottom">
		<div class="container py-lg-4">
			<div id="mission" class="row justify-content-center text-center mb-5">
				<div class="col-lg-10">
					<span class="text-uppercase text-primary font-monospace small fw-bold">Our Engineering Directive</span>
					<blockquote class="blockquote mt-3 mb-4">
						<p class="display-6 fw-bold text-dark lh-base">
							“Democratizing computer science education through accessible, structured, and pragmatic engineering curricula.”
						</p>
					</blockquote>
					<p class="lead text-secondary mx-auto" style="max-width: 800px;">
						We believe the journey from your first console log to architecting highly-available systems should not be clouded by paywalls, outdated tutorials, or abstract theoretical detachment. BytePath is engineered to turn learners into production-caliber craftsmen.
					</p>
				</div>
			</div>

			<div id="contact" class="row g-4 align-items-stretch">
				<div class="col-lg-5">
					<div class="card h-100 border rounded-4 p-4 bg-light shadow-sm">
						<h3 class="fw-bold text-dark mb-2">Get In Touch</h3>
						<p class="text-secondary small mb-4">
							Have curriculum suggestions, institutional partnership proposals, or want to contribute an open-source track? Our team responds within 24 hours.
						</p>

						<div class="d-flex flex-column gap-3 mb-4">
							<div class="d-flex align-items-center gap-3 p-3 bg-white border rounded-3">
								<div class="rounded-circle bg-primary-subtle text-primary p-2 d-flex align-items-center justify-content-center" style="width: 40px; height: 40px;">
									<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
								</div>
								<div>
									<div class="text-muted small">Direct Inquiries</div>
									<a href="mailto:contact@bytepath.dev" class="text-dark fw-semibold text-decoration-none">contact@bytepath.dev</a>
								</div>
							</div>

							<div class="d-flex align-items-center gap-3 p-3 bg-white border rounded-3">
								<div class="rounded-circle bg-primary-subtle text-primary p-2 d-flex align-items-center justify-content-center" style="width: 40px; height: 40px;">
									<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
								</div>
								<div>
									<div class="text-muted small">Hotline &amp; QC Campus</div>
									<div class="text-dark fw-semibold">+63 (9) 0123-4567</div>
								</div>
							</div>
						</div>
					</div>
				</div>

				<div class="col-lg-7">
					<div class="card h-100 border rounded-4 p-4 bg-white shadow-sm">
						<h4 class="fw-bold text-dark mb-1">Send a Direct Message</h4>
						<p class="text-secondary small mb-4">Drop your note and our dev educators will review your request.</p>

						<form @submit.prevent="handleSubmit">
							<div class="row g-3">
								<div class="col-md-6">
									<label class="form-label small fw-semibold text-dark">Developer Name</label>
									<input type="text" class="form-control" placeholder="e.g. Alex Rivera" required>
								</div>
								<div class="col-md-6">
									<label class="form-label small fw-semibold text-dark">Email Address</label>
									<input type="email" class="form-control" placeholder="alex@domain.dev" required>
								</div>
								<div class="col-12">
									<label class="form-label small fw-semibold text-dark">Track Interest</label>
									<select class="form-select">
										<option selected>General Exploration / All Tracks</option>
										<option value="1">Full-Stack Web Foundations</option>
										<option value="2">Modern Backend &amp; Distributed Systems</option>
										<option value="3">Applied Data Structures &amp; Algorithms</option>
										<option value="4">Cloud Infrastructure &amp; DevOps</option>
										<option value="5">AI &amp; Machine Learning</option>
									</select>
								</div>
								<div class="col-12">
									<label class="form-label small fw-semibold text-dark">Your Message or Question</label>
									<textarea class="form-control" rows="4" placeholder="Tell us what you're building or what learning path you need guidance with..." required></textarea>
								</div>
								<div class="col-12 text-end">
									<button type="submit" class="btn btn-primary px-4 fw-medium">
										Send Message <i class="bi bi-send ms-1"></i>
									</button>
								</div>
							</div>
						</form>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script setup>
	function handleSubmit(){
		alert('Thank you! Your message has been sent.');
	}
</script>