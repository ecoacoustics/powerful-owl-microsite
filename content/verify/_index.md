+++
title = "Whoo's Calling | Verify"
+++

<oe-verification-grid data-campaign="Powerful Owl" id="verification-grid" grid-size="1">
    <oe-verification verified="true" shortcut="y">Yes</oe-verification>
    <oe-verification verified="false" shortcut="n">No</oe-verification>
    <oe-verification verified="unsure" shortcut="u">Unsure</oe-verification>
    <oe-data-source
        slot="data-source"
        for="verification-grid"
        allow-downloads="false"
    ></oe-data-source>
</oe-verification-grid>

<div class="examples-container">
    <h2>Example Calls</h2>
    <div class="example-calls">
        <div class="card-host">
            <sl-card class="spectrogram-card">
                <div class="card-header" slot="header">
                    <h3 class="event-label">Powerful Owl (Male)</h3>
                    <oe-media-controls for="example-1"></oe-media-controls>
                </div>
                <div class="card-body">
                    <oe-annotate>
                        <oe-axes>
                            <oe-indicator>
                                <oe-spectrogram
                                    id="example-1"
                                    src="/Ninox-strenua-male.mp3"
                                    window-size="2048"
                                    window-overlap="512"
                                    mel-scale
                                ></oe-spectrogram>
                            </oe-indicator>
                        </oe-axes>
                    </oe-annotate>
                </div>
            </sl-card>
        </div>
        <div class="card-host">
            <sl-card class="spectrogram-card">
                <div class="card-header" slot="header">
                    <h3 class="event-label">Powerful Owl (Female)</h3>
                    <oe-media-controls for="example-2"></oe-media-controls>
                </div>
                <div class="card-body">
                    <oe-annotate>
                        <oe-axes>
                            <oe-indicator>
                                <oe-spectrogram
                                    id="example-2"
                                    src="/Ninox-strenua-female.mp3"
                                    window-size="2048"
                                    window-overlap="1024"
                                    mel-scale
                                ></oe-spectrogram>
                            </oe-indicator>
                        </oe-axes>
                    </oe-annotate>
                </div>
            </sl-card>
        </div>
        <div class="card-host">
            <sl-card class="spectrogram-card">
                <div class="card-header" slot="header">
                    <h3 class="event-label">Powerful Owl (Chick)</h3>
                    <oe-media-controls for="example-3"></oe-media-controls>
                </div>
                <div class="card-body">
                    <oe-annotate>
                        <oe-axes>
                            <oe-indicator>
                                <oe-spectrogram
                                    id="example-3"
                                    src="/Powerful-Owl_Ninox-strenua_chick-begging_Ed-McNabb.mp3"
                                    window-size="1024"
                                    window-overlap="128"
                                    window-function="tukey"
                                    mel-scale
                                ></oe-spectrogram>
                            </oe-indicator>
                        </oe-axes>
                    </oe-annotate>
                </div>
            </sl-card>
        </div>
</div>

<style>
.examples-container {
    margin-block: var(--micro-padding-large);
}

.example-calls {
    display: flex;
    gap: var(--micro-padding-medium);
    justify-content: space-around;
    flex-wrap: wrap;
}

.card-host {
    sl-card {
        display: block;
        height: 100%;
    }

    .card-body {
        min-width: 370px;
    }
}

h3 {
    font-size: 1.2rem;
    margin: 0;
    margin-right: 1em;
}
</style>
