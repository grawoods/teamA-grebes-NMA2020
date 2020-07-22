# teamA-grebes-NMA2020

Internal representation of self-movement normally relies on vestibular and visual (VV) inputs. When these inputs are impaired, other modes of motor processing, which may rely on motor efference copies or more noisy sensory feedback, such as proprioception and haptics, may become engaged for internal representations of running. We hypothesize that an internal representation of running is present in the absence of VV inputs. To test this, we propose to study mice in a head-fixed and dark environment, which does not provide VV inputs, but preserves some afferent and efferent signaling. Using the Stringer & Steinmetz datasets, we plan to decode movements across multiple mouse brain regions with the following specific questions in mind. 

Can self-movement (running) be decoded in a head-fixed mouse in darkness?  
Is self-movement integration distributed throughout the brain? 
What are the neuronal populations associated with motor initiation, movement speed, and sensory feedback of motion?
Data set: Stringer spontaneous (Ca2+) and external Stringer & Steinmetz (Neuropixels) during spontaneous running behaviour


Techniques:
Linear regression with a sparsity prior to identify highly tuned neuronal populations to spontaneous movement (binary) (Neuropixels, Ca2+) and movement speed (real values)
Identify the anatomical regions of highly tuned neurons using implant location and channel number of Neuropixels probes mapped onto the Allen Atlas
Identify the temporal sequence of movement control by ranking the highly tuned neurons by their signal onset time, as defined by a threshold in firing frequency
Identify populations tuned to the anticipatory and reactive phases of movement by using different temporal filters which are ahead and behind each current time step

Controls: 
We plan to use cross-validation on held-out data and make use of regularization. Further, we will use internal controls, such as comparison across brain regions. Finally, we will use external controls consisting of separate light and dark sessions. 

Keywords: population and single-unit decoding, encoding, state-space, low dimensional, latent dynamics, manifolds, spatiotemporal tuning, high-density, machine learning, neural trajectory 
