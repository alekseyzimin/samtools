ACLOCAL_AMFLAGS = -I m4
bin_PROGRAMS = samtools
lib_LIBRARIES = libbam.a bcftools/libbcf.a

AM_CPPFLAGS = -I. -D_FILE_OFFSET_BITS=64 -D_LARGEFILE64_SOURCE -D_USE_KNETFILE -D_CURSES_LIB=1
AM_LDFLAGS = -lcurses -lm -lz -lpthread


samtools_SOURCES = bam_tview.c bam_plcmd.c sam_view.c bam_rmdup.c	\
		   bam_rmdupse.c bam_mate.c bam_stat.c bam_color.c	\
		   bamtk.c kaln.c bam2bcf.c bam2bcf_indel.c errmod.c	\
		   sample.c cut_target.c phase.c bam2depth.c		\
		   padding.c bedcov.c bamshuf.c bam_tview_curses.c	\
		   bam_tview_html.c
samtools_LDADD = libbam.a bcftools/libbcf.a


libbam_a_SOURCES = bgzf.c kstring.c bam_aux.c bam.c bam_import.c	\
	            sam.c bam_index.c bam_pileup.c bam_lpileup.c	\
	            bam_md.c razf.c faidx.c bedidx.c knetfile.c		\
	            bam_sort.c sam_header.c bam_reheader.c kprobaln.c	\
	            bam_cat.c

bcftools_libbcf_a_SOURCES = bcftools/bcf.c bcftools/vcf.c		\
                             bcftools/bcfutils.c bcftools/prob1.c	\
                             bcftools/em.c bcftools/kfunc.c		\
                             bcftools/kmin.c bcftools/index.c		\
                             bcftools/fet.c bcftools/mut.c		\
                             bcftools/bcf2qcall.c bcftools/call1.c
