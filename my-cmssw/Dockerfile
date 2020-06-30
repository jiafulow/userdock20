# Use the CC7 CMSSW CVMFS image as a parent image.
FROM clelange/cc7-cmssw-cvmfs

# Set the user and working directory.
WORKDIR /home/cmsusr
USER cmsusr
ENV USER cmsusr
ENV HOME /home/cmsusr

# Run the specified command within the container.
ENTRYPOINT ["/opt/cms/entrypoint.sh"]
CMD ["/bin/zsh"]
